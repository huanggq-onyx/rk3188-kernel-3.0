EXTRA_CFLAGS += -Os
ifneq ($(CONFIG_RK_FPGA),y)
obj-y += ../plat-rk/clock.o
obj-y += clock_data.o
obj-y += ../mach-rk30/ddr.o
obj-y += ../mach-rk30/pmu.o
obj-y += ../mach-rk30/reset.o
obj-$(CONFIG_PM) += ../mach-rk30/pm.o
endif
obj-y += ../mach-rk30/common.o
CFLAGS_common.o += -DTEXT_OFFSET=$(TEXT_OFFSET)
obj-y += ../mach-rk30/devices.o
obj-y += io.o
obj-y += rk_timer.o
obj-$(CONFIG_SMP) += ../mach-rk30/platsmp.o ../mach-rk30/headsmp.o
obj-$(CONFIG_HOTPLUG_CPU) += ../mach-rk30/hotplug.o
obj-$(CONFIG_CPU_IDLE) += ../mach-rk30/cpuidle.o
obj-$(CONFIG_CPU_FREQ) += cpufreq.o
obj-$(CONFIG_DVFS) += dvfs.o
obj-y += board.o

board-$(CONFIG_MACH_RK3188_FPGA) += board-rk3188-fpga.o
board-$(CONFIG_MACH_RK3188_TB) += ../mach-rk30/board-rk3168-tb.o
board-$(CONFIG_MACH_RK3188_SDK) += board-rk3188-sdk.o
board-$(CONFIG_MACH_RK3188_LR097) += ../mach-rk30/board-rk3168-LR097.o
board-$(CONFIG_MACH_RK3188_DS1006H) += board-rk3188-ds1006h.o
board-$(CONFIG_MACH_RK3188_Q72) += board-rk3188-q72.o
board-$(CONFIG_MACH_RK3188_Q3188M) += board-rk3188-q3188m.o
board-$(CONFIG_MACH_RK3188_M7R) += board-rk3188-m7r.o
board-$(CONFIG_MACH_RK3188_A1013) += board-rk3188-a1013.o
obj-$(CONFIG_SOC_RK3188) += board.o
board-$(CONFIG_MACH_RK3188_FAC) += board-rk3188-fac.o
