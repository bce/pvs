#注释，Makefile文件的使用
ipl.bin : ipl.nas Makefile #如果制作ipl.bin文件，就要先检查一下ipl.nas和Makefile文件是否都准备好
../tools/nask.exe ipl.nas ipl.bin ipl.1st

pvsos.img : ipl.bin Makefile
../tools/edimg.exe imgin:../tools/fdimg0at.tek
wbinimg src:ipl.bin len:512 from:0 to:0 imgout:pvsos.img

生成img:
make -r pvsos.img
