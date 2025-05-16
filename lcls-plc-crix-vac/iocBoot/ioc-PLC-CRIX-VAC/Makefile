IOC_TOP=/reg/g/pcds/epics/ioc/common/ads-ioc/R1.0.0
IOC_INSTANCE_PATH := $(shell pwd)

# Set PRODUCTION_IOC to 1 to move from a testing to a production IOC:
PRODUCTION_IOC := 1

PROJECT_NAME := lcls-plc-crix-vac
PROJECT_PATH := ../../lcls-plc-crix-vac.tsproj
PLC := PLC_CRIX_VAC

PYTMC_OPTS := 
PREFIX := PLC:CRIXS:VAC

# With two $$, as in $$(IOC) below, this will be expanded in the
# environment of st.cmd:
DB_PARAMETERS := 'PREFIX=$(PREFIX):,IOCNAME=$$(IOC),IOC=$$(IOC)'

include $(IOC_TOP)/iocBoot/templates/Makefile.base
