################################################################################
# Automatically-generated file. Do not edit!
################################################################################

SHELL = cmd.exe

CG_TOOL_ROOT := D:/TI/ccs/tools/compiler/gcc-arm-none-eabi-7-2017-q4-major-win32

GEN_OPTS__FLAG := 
GEN_CMDS__FLAG := 

ORDERED_OBJS += \
"./croutine.o" \
"./event_groups.o" \
"./list.o" \
"./queue.o" \
"./tasks.o" \
"./timers.o" \
"./tm4c1294ncpdt_startup_ccs_gcc.o" \
"./drivers/buttons.o" \
"./drivers/eth_client_lwip.o" \
"./drivers/exosite_hal_lwip.o" \
"./drivers/http.o" \
"./drivers/pinout.o" \
"./portable/GCC/ARM_CM4F/port.o" \
"./portable/MemMang/heap_2.o" \
-Wl,-T"../tm4c1294ncpdt.lds" \
$(GEN_CMDS__FLAG) \

-include ../makefile.init

RM := DEL /F
RMDIR := RMDIR /S/Q

# All of the sources participating in the build are defined here
-include sources.mk
-include subdir_vars.mk
-include drivers/subdir_vars.mk
-include portable/GCC/ARM_CM4F/subdir_vars.mk
-include portable/MemMang/subdir_vars.mk
-include subdir_rules.mk
-include drivers/subdir_rules.mk
-include portable/GCC/ARM_CM4F/subdir_rules.mk
-include portable/MemMang/subdir_rules.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C55_DEPS)),)
-include $(C55_DEPS)
endif
ifneq ($(strip $(C_UPPER_DEPS)),)
-include $(C_UPPER_DEPS)
endif
ifneq ($(strip $(S67_DEPS)),)
-include $(S67_DEPS)
endif
ifneq ($(strip $(S62_DEPS)),)
-include $(S62_DEPS)
endif
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(OPT_DEPS)),)
-include $(OPT_DEPS)
endif
ifneq ($(strip $(C??_DEPS)),)
-include $(C??_DEPS)
endif
ifneq ($(strip $(ASM_UPPER_DEPS)),)
-include $(ASM_UPPER_DEPS)
endif
ifneq ($(strip $(S??_DEPS)),)
-include $(S??_DEPS)
endif
ifneq ($(strip $(C64_DEPS)),)
-include $(C64_DEPS)
endif
ifneq ($(strip $(CXX_DEPS)),)
-include $(CXX_DEPS)
endif
ifneq ($(strip $(S64_DEPS)),)
-include $(S64_DEPS)
endif
ifneq ($(strip $(INO_DEPS)),)
-include $(INO_DEPS)
endif
ifneq ($(strip $(CLA_DEPS)),)
-include $(CLA_DEPS)
endif
ifneq ($(strip $(S55_DEPS)),)
-include $(S55_DEPS)
endif
ifneq ($(strip $(SV7A_DEPS)),)
-include $(SV7A_DEPS)
endif
ifneq ($(strip $(C62_DEPS)),)
-include $(C62_DEPS)
endif
ifneq ($(strip $(C67_DEPS)),)
-include $(C67_DEPS)
endif
ifneq ($(strip $(PDE_DEPS)),)
-include $(PDE_DEPS)
endif
ifneq ($(strip $(K_DEPS)),)
-include $(K_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
ifneq ($(strip $(CC_DEPS)),)
-include $(CC_DEPS)
endif
ifneq ($(strip $(C++_DEPS)),)
-include $(C++_DEPS)
endif
ifneq ($(strip $(C43_DEPS)),)
-include $(C43_DEPS)
endif
ifneq ($(strip $(S43_DEPS)),)
-include $(S43_DEPS)
endif
ifneq ($(strip $(ASM_DEPS)),)
-include $(ASM_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(CPP_DEPS)),)
-include $(CPP_DEPS)
endif
ifneq ($(strip $(SA_DEPS)),)
-include $(SA_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXE_OUTPUTS += \
TivaC-TM4C-FreeRTOS.out \

EXE_OUTPUTS__QUOTED += \
"TivaC-TM4C-FreeRTOS.out" \

BIN_OUTPUTS += \
TivaC-TM4C-FreeRTOS.hex \

BIN_OUTPUTS__QUOTED += \
"TivaC-TM4C-FreeRTOS.hex" \


# All Target
all: $(OBJS) $(LDS_SRCS) $(A_SRCS) $(GEN_CMDS)
	@$(MAKE) --no-print-directory -Onone "TivaC-TM4C-FreeRTOS.out"

# Tool invocations
TivaC-TM4C-FreeRTOS.out: $(OBJS) $(LDS_SRCS) $(A_SRCS) $(GEN_CMDS)
	@echo 'Building target: "$@"'
	@echo 'Invoking: GNU Linker'
	"D:/TI/ccs/tools/compiler/gcc-arm-none-eabi-7-2017-q4-major-win32/bin/arm-none-eabi-gcc-7.2.1.exe" -DPART_TM4C1294NCPDT -Dgcc -Os -ffunction-sections -fdata-sections -fsingle-precision-constant -g -gdwarf-3 -gstrict-dwarf -Wall -specs="nosys.specs" -march=armv7e-m -mthumb -mfloat-abi=hard -mfpu=fpv4-sp-d16 -Wl,-Map,"TivaC-TM4C-FreeRTOS.map" -Wl,--gc-sections -o"TivaC-TM4C-FreeRTOS.out" $(ORDERED_OBJS) $(A_SRCS)
	@echo 'Finished building target: "$@"'
	@echo ' '

TivaC-TM4C-FreeRTOS.hex: $(EXE_OUTPUTS)
	@echo 'Building files: $(strip $(EXE_OUTPUTS__QUOTED))'
	@echo 'Invoking: GNU Objcopy Utility'
	"D:/TI/ccs/tools/compiler/gcc-arm-none-eabi-7-2017-q4-major-win32/bin/arm-none-eabi-objcopy.exe"  $(EXE_OUTPUTS__QUOTED) "TivaC-TM4C-FreeRTOS.hex"
	@echo 'Finished building: $(strip $(EXE_OUTPUTS__QUOTED))'
	@echo ' '

# Other Targets
clean:
	-$(RM) $(BIN_OUTPUTS__QUOTED)$(EXE_OUTPUTS__QUOTED)
	-$(RM) "croutine.o" "event_groups.o" "list.o" "queue.o" "tasks.o" "timers.o" "tm4c1294ncpdt_startup_ccs_gcc.o" "drivers\buttons.o" "drivers\eth_client_lwip.o" "drivers\exosite_hal_lwip.o" "drivers\http.o" "drivers\pinout.o" "portable\GCC\ARM_CM4F\port.o" "portable\MemMang\heap_2.o" 
	-$(RM) "croutine.d" "event_groups.d" "list.d" "queue.d" "tasks.d" "timers.d" "tm4c1294ncpdt_startup_ccs_gcc.d" "drivers\buttons.d" "drivers\eth_client_lwip.d" "drivers\exosite_hal_lwip.d" "drivers\http.d" "drivers\pinout.d" "portable\GCC\ARM_CM4F\port.d" "portable\MemMang\heap_2.d" 
	-@echo 'Finished clean'
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets

