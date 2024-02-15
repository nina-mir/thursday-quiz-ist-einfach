# Ubuntu-setup-virtualbox
### A guide to install Ubuntu OS in VirtualBox
*The information in this guide is based on the work/materials by Robert Bierman and Andrew Scott of SF State CS Dept re: CSC 317 course. (Additional information is included from other online sources.)*
***
### A short exaplnation from IBM:
#### What is virtualization?
source: https://www.ibm.com/topics/virtualization

Virtualization is a process that allows for more efficient utilization of physical computer hardware and is the foundation of cloud computing.

Virtualization uses software to create an abstraction layer over computer hardware that allows the hardware elements of a single computer—processors, memory, storage and more—to be divided into multiple virtual computers, commonly called virtual machines (VMs). Each VM runs its own operating system (OS) and behaves like an independent computer, even though it is running on just a portion of the actual underlying computer hardware.

It follows that virtualization enables more efficient utilization of physical computer hardware and allows a greater return on an organization’s hardware investment.

Today, virtualization is a standard practice in enterprise IT architecture. It is also the technology that drives cloud computing economics. Virtualization enables cloud providers to serve users with their existing physical computer hardware; it enables cloud users to purchase only the computing resources they need when they need it, and to scale those resources cost-effectively as their workloads grow.
***
Now read the guide: 
This guid has two different sections: [intel](#first) architecture and [MacBook M1/M2](#second). Refer to the section that matches your computer's CPU architecture, please. 

### <a id="first">Intel 64bit</a>

**Step. 1** download and install VirtualBox version VirtualBox 6.1.20 (released April 20 2021) + Package Extension file from the following link. Refer to the image below from the same link for more info.

Link: https://www.virtualbox.org/wiki/Download_Old_Builds_6_1

<img src="images-setup/virtualbox-6.1.2.png" width="400">

First, install VirtualBox on your machine. 

**Note for Mac users with an Intel CPU**: the installation step may fail for you due to a known issue with the hardware. In that case, you need to refer to slides 6 & 7 on the PDF file included in this repo  <a href="317 Unit 01 - Setup v4.pdf">"317 Unit 01 - Setup v4.pdf"</a>

Upon a successfulinstallation, open VirtualBox program on your computer. You should see the following image. 

<img src="images-setup/vbox-welcome.png" width="500">

Click on **Tools**. Then, click on File>Preferneces>Extensions. Now, click on the plus button to add the Extension Package file that you downloaded earlier. Press OK and exit. 

**Step.2**
In this step, we will install Ubuntu 22.04 LTS	Jammy Jellyfish using the VirtualBox. First, you need to downloand an OVA file containing an image of Ubuntu OS that has VSCode and Node.js already installed on it from this link: https://sfsu.app.box.com/v/csc317webdevova 

Note: It is a large file of 6.9 GB. It will take minutes to hours depending on your internet connection to download. 

The **USER NAME** and **PASSWORD** of the resultant Ubuntu OS (you'll need these crednetials to login!): 

* username = student
* password = student

After the OVA file is downloaded. Go the main menu of Virtualbox. Now, press on **Import** button on the right side as seen below.

<img src="images-setup/Import-virtual-box.png" width="500">

Now, press on the folder button as seen below and select the OVA file on your hard drive. Then, press **Next**.

<img src="images-setup/import_menue.png" width="500">

Do not change any default values in this step but pay attentin to the displayed information about the to-be-created virtual machine.
The image below is an example.

<img src="images-setup/appliance_settings_VM.png" width="500">

Press **import**.
This step may take a few minutes.

<img src="images-setup/Screenshot from 2024-01-31 13-06-07.png" width="500">

**Step.3**
If all the previous steps are successfully completed, you should see a WebDec2023 **_machine_** on your VirtualBox menue. Click on it!

<img src="images-setup/press_on_new_machine.png" width="500">

After selecting you new _machine_, you should see a similar menue. Click on **_Start_** button to boot your Ubuntu machine.
After Ubuntu is booted, enter the password provided above: student. 
Now look around Ubuntu and figure things out! 

<img src="images-setup/run_the_VM.png" width="500">

### <a id="second">MacBook M1, M2 chipset</a>

  

Folks with an ARM cpu architecture cannot use VirtualBox to install Ubuntu OS. You have other options. 

**Option. 1** -- **buy Parallels**. It is about $50 for students. https://www.parallels.com/products/desktop/buy/?full

Watch the following video on YouTube on how to **install Ubuntu** on your Macbook. The video assumed you have already installed Parallels. 

link: https://youtu.be/EiO_CHfSn2s?si=_XTa1OQzeMoMnmLv

**Option. 2** -- use a free open-source application like UTM. You can download it for free or buy it from the Apple store for $10.

Follow this link to download it: https://mac.getutm.app/

Installation guide: https://docs.getutm.app/guides/ubuntu/

**Other sources that could help**: 
_text _ -- https://jun1okamura.medium.com/install-ubuntu-on-mac-m1-powered-by-utm-499aba3ba7e9

_video/text_ -- https://techyrick.com/installing-ubuntu-on-utm-apple-m1-m2/

### Note: If you cannot install Ubuntu OS on your computer you can always checkout a Windows laptop from the library and follows the instructions for Intel chips above. 











