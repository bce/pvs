#ÃüÁî
default:
	../tools/make.exe img
img :
	../tools/make.exe -r pvsos.img

clean:
	-del pvsos.img

pvsos.img: helloos.nas Makefile
	..\tools\nask.exe helloos.nas pvsos.img