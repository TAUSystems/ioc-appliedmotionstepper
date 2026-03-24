TOP=../..

include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

# The following are used for debugging messages.
USR_CXXFLAGS += -DDEBUG

#==================================================
# build a support library

LIBRARY_IOC += motorAppliedMotionStepper

# xxxRecord.h will be created from xxxRecord.dbd
#DBDINC += xxxRecord
# install motorAppliedMotionStepper.dbd into <top>/dbd
DBD += motorAppliedMotionStepper.dbd

# specify all source files to be compiled and added to the library
motorAppliedMotionStepper_SRCS += StepperDriver.cpp

motorAppliedMotionStepper_LIBS += motor asyn
motorAppliedMotionStepper_LIBS += $(EPICS_BASE_IOC_LIBS)

#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

