################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32F4xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
TUT_STM32F4_DHT11_22_DS18B20.elf \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
TUT_STM32F4_DHT11_22_DS18B20.list \


# All Target
all: TUT_STM32F4_DHT11_22_DS18B20.elf secondary-outputs

# Tool invocations
TUT_STM32F4_DHT11_22_DS18B20.elf: $(OBJS) $(USER_OBJS) C:\Users\Elnaz\Desktop\STM32F4_DHT11_\STM32F446RETX_FLASH.ld
	arm-none-eabi-gcc -o "TUT_STM32F4_DHT11_22_DS18B20.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m4 -T"C:\Users\Elnaz\Desktop\STM32F4_DHT11_\STM32F446RETX_FLASH.ld" --specs=nosys.specs -Wl,-Map="TUT_STM32F4_DHT11_22_DS18B20.map" -Wl,--gc-sections -static --specs=nano.specs -mfpu=fpv4-sp-d16 -mfloat-abi=hard -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

TUT_STM32F4_DHT11_22_DS18B20.list: $(EXECUTABLES)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "TUT_STM32F4_DHT11_22_DS18B20.list"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) *
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
