EG ?= simple_CPU

DISTRO ?= /home/rishi/Documents/My_Project/CODE_HERE/8bit_simple_cpu/

TOPFILE   ?= $(DISTRO)/Example_Programs/$(EG)/src_BSV/SimpleCPU.bsv
TOPMODULE ?= mkSimpleCPU

BSC_COMP_FLAGS = -elab -keep-fires -aggressive-conditions -no-warn-action-shadowing
BSC_LINK_FLAGS = -keep-fires
BSC_PATHS = -p $(DISTRO)/Example_Programs/$(EG)/src_BSV:$(DISTRO)/Example_Programs/Common:%/Prelude:%/Libraries

BSIM_DIRS = -simdir build_bsim -bdir build_bsim -info-dir build_bsim
BSIM_EXE = $(TOPMODULE)_bsim
