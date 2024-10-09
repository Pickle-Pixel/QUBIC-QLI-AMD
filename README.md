## **Install ROCm 6.1.1**
- Official ROCm https://rocm.docs.amd.com/projects/install-on-linux/en/docs-6.1.1/how-to/amdgpu-install.html


## **Steps to get Install ROCm 6.1.1**
- run the following commands on terminal
- ```sudo apt update```
- ```wget https://repo.radeon.com/amdgpu-install/6.1.1/ubuntu/jammy/amdgpu-install_6.1.60101-1_all.deb```
- ```sudo apt install ./amdgpu-install_6.1.60101-1_all.deb```
- ```sudo amdgpu-install```
- now check if the GPU is actually identified and working with this command ```rocm-smi``` and it should display GPUs information.


## **ZLUDA Installation**
- Step #1 Navigate to the folder where qli-Client is set up and installed.
- Step #2 ```wget https://github.com/vosen/ZLUDA/releases/download/v3/zluda-3-linux.tar.gz```
- Step #3 ```tar -xzvf zluda-3-linux.tar.gz```
- Step #4 Create a script called gpu.sh and it should look like this from the inside ```LD_LIBRARY_PATH="/path/to/zluda/:$LD_LIBRARY_PATH" ./qli-Client```
- Note: make sure to change `/path/to/zluda/` in the script to point to the folder named zluda that you extracted in step #3

## **START MINING!**
- we have to make the script executable ```chmod +x gpu.sh```
- now run the script with ```./gpu.sh``` and watch your AMD GPUs work!

## **Personal Experience*
- I have RX 7900XTX and it currently gets 130-140 it/s on QLI
- 
