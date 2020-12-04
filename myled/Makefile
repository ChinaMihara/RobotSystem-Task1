#SPDX-License-Identifier: GPL-2.0
#
#	Copyright (C) 2020 Ryuichi Ueda. All right reserved.
#

obj-m := myled.o

myled.ko: myled.c
	make -C /usr/src/linux-headers-`uname -r` M=`pwd` V=1 modules

clean:
	make -C /usr/src/linux-headers-`uname -r` M=`pwd` V=1 clean
