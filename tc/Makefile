################################################################################
#
# Intel SmartPHY DSL PCIe TC driver
# Copyright(c) 2016 Intel Corporation.
#
# This program is free software; you can redistribute it and/or modify it
# under the terms and conditions of the GNU General Public License,
# version 2, as published by the Free Software Foundation.
#
# This program is distributed in the hope it will be useful, but WITHOUT
# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
# FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for
# more details.
#
# You should have received a copy of the GNU General Public License along with
# this program; if not, write to the Free Software Foundation, Inc.,
# 51 Franklin St - Fifth Floor, Boston, MA 02110-1301 USA.
#
# The full GNU General Public License is included in this distribution in
# the file called "COPYING".
#
################################################################################

#
# Makefile for the Intel(R) SmartPHY TC driver
#

obj-$(CONFIG_VRX518_TC) += vrx518_tc.o
vrx518_tc-objs := ptm_tc.o atm_tc.o tc_api.o tc_proc.o tc_main.o

ifneq ($(CONFIG_VRX518_CPU),)
vrx518_tc-objs += platform/sw_plat.o
endif
ifneq ($(CONFIG_VRX518_GRX500),)
vrx518_tc-objs += platform/grx500_plat.o
endif
ifneq ($(CONFIG_VRX518_DC_DP),)
vrx518_tc-objs += platform/dcdp_plat.o
endif
