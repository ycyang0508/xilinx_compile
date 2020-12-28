# xilinx_compile

####################
# .bashrc

export CDS_INST_DIR=/home/ycyang/cadence/installs/XCELIUM2003

export LD_LIBRARY_PATH=${CDS_INST_DIR}/tools.lnx86/lib:$LD_LIBRARY_PATH

export PATH=${CDS_INST_DIR}/bin:${CDS_INST_DIR}/tools.lnx86/bin:$PATH

export GCC_SIM_EXE_PATH=/home/ycyang/cadence/installs/XCELIUM2003/tools.lnx86/systemc/gcc/bin/64bit/

####################

####################
# create symolic link 
cd /home/ycyang/cadence/installs/XCELIUM2003/

sudo ln -s ./tools/systemc/ ./

####################
# 
vivado -mode tcl 

compile_simlib -dir /home/ycyang/working/xilinx_test/sim_lib -simulator xcelium -verbose 

####################




