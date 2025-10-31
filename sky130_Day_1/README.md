# Sky130 Day 1 - Inception of open-source EDA, OpenLANE and Sky130 PDK  

#How to talk to computers:  

> Introduction to QFN-48 Package, chip, pads, core, die and IPs  
Image below shows the Arduino board with a IC which is the core of the board which is a microcontroller:  
![Arduino Image](./assets/arduino_image.png)  

Below image describes the system view of the Arduino board.  
![Arduino System View](./assets/arduino_system_view.png)  

![QFN View](./assets/qfn_view.png)  

![QFN Package with Chip](./assets/qfn_package_with_chip.png)  

![Chip View](./assets/chip_view.png)  

![Chip with Cores and Foundry IPs and Macros](./assets/chip_with_cores_and_foundry_IPs_and_macros.png)  


> Introduction to RISC-V  

![RISC-V Architecture Introduction](./assets/RISCV_arch_intro.png)  

> From Software Applications to Hardware  

![Chip Flow Program to Chip](./assets/chip_flow_program_to_chip.png)  

![Chip Flow Low Level](./assets/chip_flow_low_level.png)  



#####################
#change the main directory
cd Desktop

#change the directory
cd work/tools/

#open the directory
ls -ltr

#change the directory
cd openlane_working_dir

#open the directory
ls -lrt

#change the directory
cd pdks


work_dir_view.png



libs_ref_tech.png


#Change directory to openlane flow directory
cd Desktop/work/tools/openlane_working_dir/openlane

#alias docker='docker run -it -v $(pwd):/openLANE_flow -v $PDK_ROOT:$PDK_ROOT -e PDK_ROOT=$PDK_ROOT -u $(id -u $USER):$(id -g $USER) efabless/openlane:v0.21'
#Since we have aliased the long command to 'docker' we can invoke the OpenLANE flow docker sub-system by just running this command
docker

## Now that we have entered the OpenLANE flow contained docker sub-system we can invoke the OpenLANE flow in the Interactive mode using the following command
./flow.tcl -interactive

#activates OpenLane’s Tcl package (version 0.9)
package require openlane 0.9 (in the OpenLANE environment)

#initial setup stage of the OpenLane physical design flow
prep -design picorv32a

docker_Run_openlane.png


prep_design.png

view_after_prep.png

merged_lef1.png

merged_lef2.png




run_synthesis.png

printing_synth_stats.png

printing_synth_stats2.png

printing_synth_stats3.png

synth_done.png

synth_file_ls.png

report_view.png
###########################



#Soc Design and OpenLANE  
> Introduction to all components of open-source digital asic design  
> Simplified RTL2GDS flow  
> Introduction to OpenLANE and Strive chipsets  
> Introduction to OpenLANE detailed ASIC design flow  

#Get familiar to Open-source EDA Tools  
> OpenLANE Directory structure in detail  
> Design Preparation Step  
> Review files after design prep and run synthesis  
> OpenLANE Project Git Link Description  
> Steps to characterize synthesis results  

