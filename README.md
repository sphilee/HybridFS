         Hybridfs v1.0

WHAT IS THIS?
   Hybrid file system�̶� ssd storage�� hdd storage�� �ϳ��� ����̺�� �����Ͽ� ������ �ý����̴�.

ON WHAT HARDWARE DOES IT RUN?
   OS : Linux 12.04.5 LTS
   Kernel : Linux-2.6.35
   SSD : Samsung 850 PRO 128GB
   HDD : Samsung 500GB 7200RPM

DOCUMENTATION:
   1. ������ ������ �о�� ũ�Ⱑ ū ������ HDD�� ���� ������ SSD�� �Ű��ִ� ����� �Ѵ�.
   2. SSD�� �ִ� symbolic file link�� ����Ͽ� HDD �� �ִ� ������ �����ϰ� �Ѵ�.
   3. �÷��׸� ����� ���ֽ� �߻��ϴ� ���� ���� ��û�� ��� ���� �������� ��û�� ��ȿȭ �ϰ� ���� ���� �� ���ָ� �����ϴ� ����� ����Ÿ ���ֽ� ���Ἲ�� �����Ѵ�.
   4. HDD���� ���� IO�� �����ϰ� Embedded attributes�� �̿��ϴ� Replicating attributes ����� ����Ѵ�.

SOFTWARE REQUIREMENTS:
   fuse-tutorial-2016-03-25/src/bbfs.c
   fuse-tutorial-2016-03-25/src/log.c
   fuse-tutorial-2016-03-25/src/log.h
   fuse-tutorial-2016-03-25/src/Makefile

COMPILING:
   1) make
   2) ./bbfs /home/tim/Downloads/tmp/ssd /home/tim/Downloads/tmp/hybridfs/