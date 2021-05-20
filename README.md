# OAIUSRPN321
Files updated in order to make Ettus USRP N321 with OAI code
In order to make OAI code work with USRP N321 please make sure to replace these files for the original OAI develop branch. Configuration files used are also included and prepared to work with USRP B210 as eNB and N321 as gNB.
# FOLDERS WHERE SCRIPTS ARE:

cmake_targets/build_oai
# modified UHD installation (from source) 
#443# install_usrp_uhd_driver-> install_usrp_uhd_driver_from_source

cmake_targets/tools/build_helper
# changed the UHD version installed to UHD 3.15
#262# git checkout tags/v3.13.0.2 -> git checkout tags/v3.15.0.0

targets/ARCH/USRP/USERSPACE/LIB/usrp_lib.cpp
# modified clock frequency to make it compatible with USRP N321
#1098# usrp_master_clock = 122.88e6 -> usrp_master_clock = 254.76e6;
