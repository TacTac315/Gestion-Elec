################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include src/subdir.mk
-include Project_Settings/Startup_Code/subdir.mk
-include Project_Settings/Linker_Files/subdir.mk
-include FreeMaster_MPC57xxx/src_platforms/MPC57xx/subdir.mk
-include FreeMaster_MPC57xxx/src_common/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
SECONDARY_SIZE += \
PMSM_TGN002_cde_Uf_etudiant.siz \


# All Target
all: PMSM_TGN002_cde_Uf_etudiant.elf secondary-outputs

# Tool invocations
PMSM_TGN002_cde_Uf_etudiant.elf: $(OBJS) C:/Users/adminaboyer/alex/2023-24/BE_Elec_auto/Workspace/PMSM_TGN002_cde_Uf_etudiant/Project_Settings/Linker_Files/57xx_flash.ld $(OSPT) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: Standard S32DS C Linker'
	powerpc-eabivle-gcc -o "PMSM_TGN002_cde_Uf_etudiant.elf" "@PMSM_TGN002_cde_Uf_etudiant.args"  $(USER_OBJS)  $(OSPT)
	@echo 'Finished building target: $@'
	@echo ' '

PMSM_TGN002_cde_Uf_etudiant.siz: PMSM_TGN002_cde_Uf_etudiant.elf
	@echo 'Invoking: Standard S32DS Print Size'
	powerpc-eabivle-size --format=berkeley PMSM_TGN002_cde_Uf_etudiant.elf
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) ./*
	-@echo ' '

secondary-outputs: $(SECONDARY_SIZE)

.PHONY: all clean dependents

-include ../makefile.targets
