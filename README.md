#HybridFS

##WHAT IS THIS?
   Hybrid file system이란 ssd storage와 hdd storage를 하나의 드라이브로 통합하여 적용한 시스템이다.

##ON WHAT HARDWARE DOES IT RUN?
   + OS : Linux 12.04.5 LTS
   + Kernel : Linux-2.6.35
   + SSD : Samsung 850 PRO 128GB
   + HDD : Samsung 500GB 7200RPM

##DOCUMENTATION:
   1. 파일의 정보를 읽어와 크기가 큰 파일은 HDD로 작은 파일은 SSD로 옮겨주는 기능을 한다.
   2. SSD에 있는 symbolic file link를 사용하여 HDD 에 있는 파일을 참조하게 한다.
   3. 플래그를 사용해 이주시 발생하는 파일 쓰기 요청의 경우 현재 이주중인 요청을 무효화 하고 파일 쓰기 후 이주를 실행하는 방식의 데이타 이주시 무결성을 지원한다.
   4. HDD로의 작은 IO를 제거하고 Embedded attributes를 이용하는 Replicating attributes 방식을 사용한다.

##SOFTWARE REQUIREMENTS:
   + fuse-tutorial-2016-03-25/src/bbfs.c
   + fuse-tutorial-2016-03-25/src/log.c
   + fuse-tutorial-2016-03-25/src/log.h
   + fuse-tutorial-2016-03-25/src/Makefile

##COMPILING:
   1. make
   2. ./bbfs /home/tim/Downloads/tmp/ssd /home/tim/Downloads/tmp/hybridfs/
