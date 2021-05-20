# OAIUSRPN321
Files updated in order to make Ettus USRP N321 with OAI code
In order to make OAI code work with USRP N321 please make sure to replace these files for the original OAI develop branch. Configuration files used are also included and prepared to work with USRP B210 as eNB and N321 as gNB.
# FOLDERS WHERE SCRIPTS ARE:

# modified UHD installation (from source) 
cmake_targets/build_oai

#443# install_usrp_uhd_driver-> install_usrp_uhd_driver_from_source

# changed the UHD version installed to UHD 3.15
cmake_targets/tools/build_helper

#262# git checkout tags/v3.13.0.2 -> git checkout tags/v3.15.0.0

# modified clock frequency to make it compatible with USRP N321
targets/ARCH/USRP/USERSPACE/LIB/usrp_lib.cpp

#1098# usrp_master_clock = 122.88e6 -> usrp_master_clock = 254.76e6;

# OAI_XX are configuration files used
