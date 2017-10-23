# arch/arm/mach-s5pv210/Makefile
#
# Copyright (c) 2010 Samsung Electronics Co., Ltd.
#		http://www.samsung.com/
#
# Licensed under GPLv2

obj-y				:=
obj-m				:=
obj-n				:=
obj-				:=

# Core support for S5PV210 system

obj-$(CONFIG_CPU_S5PV210)	+= cpu.o init.o clock.o dma.o
obj-$(CONFIG_S5PV210_PM)	+= pm.o sleep.o
obj-$(CONFIG_CPU_FREQ)		+= cpufreq.o

obj-$(CONFIG_S5PV210_POWER_DOMAIN)	+= power-domain.o
obj-$(CONFIG_S5PV210_CORESIGHT) += coresight.o

# machine support

obj-$(CONFIG_MACH_HERRING)	+= board-herring/
obj-$(CONFIG_MACH_ARIES)	+= board-aries/
obj-$(CONFIG_MACH_P1)		+= board-p1/

# device support

obj-y				+= dev-audio.o
obj-y				+= dev-fiqdbg.o
obj-$(CONFIG_S3C64XX_DEV_SPI)	+= dev-spi.o

obj-$(CONFIG_S5P_ADC) += adc.o

obj-y += setup-dev/

obj-$(CONFIG_SAMSUNG_GALAXYS4G_TELUS_VERSION)	+= cg2900_devices.o

obj-$(CONFIG_CPU_IDLE)		+= cpuidle.o
obj-$(CONFIG_CPU_FREQ)		+= dev-cpufreq.o
obj-$(CONFIG_FORCE_FAST_CHARGE) += fastchg.o
