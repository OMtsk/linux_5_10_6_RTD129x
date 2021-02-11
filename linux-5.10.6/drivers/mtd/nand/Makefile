# SPDX-License-Identifier: GPL-2.0

nandcore-objs := core.o bbt.o
obj-$(CONFIG_MTD_NAND_CORE) += nandcore.o

obj-y	+= onenand/
obj-y	+= raw/
obj-y	+= spi/

nand-objs := rtk_nand.o nand_base_rtk.o
nandcore-$(CONFIG_MTD_NAND_ECC) += ecc.o
