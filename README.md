# amd-opencl-popos
Collection of information for installing OpenCL proprietary drivers from AMD on kernel 5.8 - PopOS 20.04 LTS

Endedup installing Ubuntu instead

When installing, the DKMS firmware will fail on the 5.8 kernel used in PopOS


sudo apt install linux-headers


sudo apt install linux-generic
sudo nano /etc/default/grub
->Change GRUB_DEFAULT=0 to GRUB_DEFAULT=1

You can also change the timeout to 5 and default from "hidden" to "menu"
reeeeboot


sudo apt remove linux-headers-5.8.0-41-generic
sudo apt remove linux-image-5.8.0-41-generic

DRIVER GUIDE:
./amdgpu-install --opencl=legacy --headless
