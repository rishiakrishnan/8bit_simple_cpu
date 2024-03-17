EG ?= simple_CPU

# Directory containing the Bluespec Training distribution directory
DISTRO ?= /home/rishi/Documents/My_Project/CODE_HERE/8bit_simple_cpu/

# Set this to the command that invokes your Verilog simulator
# VSIM ?= iverilog
VSIM ?= cvc
# VSIM ?= cver
# VSIM ?= vcsi
# VSIM ?= vcs
# VSIM ?= modelsim
# VSIM ?= ncsim
# VSIM ?= ncverilog
# ================================================================

TOPFILE   ?= $(DISTRO)/Example_Programs/$(EG)/src_BSV/SimpleCPU.bsv
TOPMODULE ?= mkSimpleCPU
