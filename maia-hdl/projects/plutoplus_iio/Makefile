####################################################################################
## Copyright (c) 2018 - 2021 Analog Devices, Inc.
### SPDX short identifier: BSD-1-Clause
####################################################################################

PROJECT_NAME := plutoplus

M_DEPS += system_project.tcl
M_DEPS += system_bd.tcl

M_DEPS += ../../adi-hdl/library/common/ad_iobuf.v
M_DEPS += ../../adi-hdl/library/common/ad_bus_mux.v
M_DEPS += ../../adi-hdl/library/axi_ad9361/axi_ad9361_delay.tcl
M_DEPS += ip_cores

LIB_DEPS += axi_ad9361
LIB_DEPS += axi_dmac
LIB_DEPS += util_pack/util_cpack2
LIB_DEPS += util_pack/util_upack2

include ../../adi-hdl/projects/scripts/project-xilinx.mk

ip_cores:
	$(MAKE) -C ../../ip

.PHONY: ip_cores
