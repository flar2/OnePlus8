# SPDX-License-Identifier: GPL-2.0-only

# auto-detect subdirs
ifeq ($(CONFIG_ARCH_KONA), y)
ifeq ($(CONFIG_ARCH_ONEPLUS8PRO), y)
include $(srctree)/techpack/display/config/op8prodisp.conf
else
include $(srctree)/techpack/display/config/konadisp.conf
endif
endif

ifeq ($(CONFIG_ARCH_KONA), y)
ifeq ($(CONFIG_ARCH_ONEPLUS8PRO), y)
LINUXINCLUDE    += -include $(srctree)/techpack/display/config/op8prodispconf.h
else
LINUXINCLUDE    += -include $(srctree)/techpack/display/config/konadispconf.h
endif
endif

ifeq ($(CONFIG_ARCH_LITO), y)
include $(srctree)/techpack/display/config/saipdisp.conf
endif

ifeq ($(CONFIG_ARCH_LITO), y)
LINUXINCLUDE    += -include $(srctree)/techpack/display/config/saipdispconf.h
endif

ifeq ($(CONFIG_ARCH_BENGAL), y)
include $(srctree)/techpack/display/config/bengaldisp.conf
endif

ifeq ($(CONFIG_ARCH_BENGAL), y)
LINUXINCLUDE    += -include $(srctree)/techpack/display/config/bengaldispconf.h
endif

obj-$(CONFIG_DRM_MSM) += msm/
obj-$(CONFIG_MSM_SDE_ROTATOR) += rotator/
obj-$(CONFIG_QCOM_MDSS_PLL) += pll/
