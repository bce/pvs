#ע�ͣ�Makefile�ļ���ʹ��
ipl.bin : ipl.nas Makefile #�������ipl.bin�ļ�����Ҫ�ȼ��һ��ipl.nas��Makefile�ļ��Ƿ�׼����
../tools/nask.exe ipl.nas ipl.bin ipl.1st

pvsos.img : ipl.bin Makefile
../tools/edimg.exe imgin:../tools/fdimg0at.tek
wbinimg src:ipl.bin len:512 from:0 to:0 imgout:pvsos.img

����img:
make -r pvsos.img
