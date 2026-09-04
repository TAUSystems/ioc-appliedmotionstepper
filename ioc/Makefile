TOP = .
include $(TOP)/configure/CONFIG

DIRS += configure
DIRS += iocApp

# All dirs except configure depend on configure
$(foreach dir, $(filter-out configure, $(DIRS)), \
    $(eval $(dir)_DEPEND_DIRS += configure))

include $(TOP)/configure/RULES_TOP
