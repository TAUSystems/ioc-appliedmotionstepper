TOP = .
include $(TOP)/configure/CONFIG

DIRS += configure
DIRS += motorAppliedMotionStepperApp
DIRS += iocApp

# All dirs except configure depend on configure
$(foreach dir, $(filter-out configure, $(DIRS)), \
    $(eval $(dir)_DEPEND_DIRS += configure))

# Add any additional dependency rules here:
iocApp_DEPEND_DIRS += motorAppliedMotionStepperApp

include $(TOP)/configure/RULES_TOP
