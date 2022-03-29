Catapult HLS Tool Use
=====================

# Installation
  At Princeton, you have access to the catapult tool via 
  ```bash 
  export PATH="/usr/licensed/MentorGraphics2021/Catapult_Synthesis_10.6a/Mgc_home/bin:$PATH"
  ```
  The License can be obtain from 
  ```bash 
  export MGLS_LICENSE_FILE="/usr/licensed/licenses/mentorgraphics.license.dat"
  ```
# Use the Catapult in GUI
  command to open the catapult HLS tool
  ```bash 
  catapult -product ultra
  ```
# Library Needed
  ## SystemC (2.3.1)
  Install it through the github repo of the [systemC](https://github.com/accellera-official/systemc)
  ```bash
  cmake .. -DCMAKE_CXX_STANDARD=11 -DCAMKE_INSTALL_PREFIX=/u/xxx/local/systemc-2.3.1
  export LD_LIBRARY_PATH="/u/huaixil/local/systemc-2.3.1/lib64:$LD_LIBRARY_PATH"
  ```
  ## Boost (1.55.0)
  The version we need is 1.55.0 for FlexASR
  ```bash
  wget http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.55/boost1.55_1.55.0.orig.tar.bz2
  tar -xvf boost1.55_1.55.0.orig.tar.bz2
  ./bootstrap.sh
  ./b2 install --prefix=/u/huaixil/local/boost-1.55.0
  ```
