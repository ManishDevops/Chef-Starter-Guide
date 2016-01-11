###Chef Workstation
One chef server can have one or more workstations. Workstation is used to create, test, manage and upload cookbooks. These cookbooks are uploaded to chef server. Before setting up workstation, please ensure that you are using one of the following machines

|S.No.|Platform|Version|
|:---|:----|:----|
|1|Fedora|current non-EOL releases|
|2|Mac OS X|10.8, 10.9, 10.10|
|3|Red Hat Enterprise Linux|6.x, 7.x|
|4|Ubuntu|12.04, 14.04|
|5|Microsoft Windows|7, 8, 8.1, Server 2012|

Click [here](https://docs.chef.io/supported_platforms.html) to know more about supported platforms.

### Chef Workstation Installation
Many developers use Chef Management Console in this process. This will make your process easier and you will get a webui but it is a Featured Component. If you want to use Chef Management Console then you can use 25 nodes for free and to use more than 25 nodes, you will have to purchase license.I am not going to use Chef Management Console in my process.

I am using a windows machine(my personal laptop) as workstation.

You need to follow following steps to install workstation.

    1. Download Chef Development Kit
    2. Install Chef Development Kit
    3. Download chef-repo
    4. Configure chef-repo
    5. Configure knife.rb
    
##### 1. Download Chef Development Kit
Go to [this](https://downloads.chef.io/chef-dk/) link and select chef dk according to your workstation machine. 


##### 2. Install Chef Development Kit
Follow the steps in the installer and install the Chef development kit to your machine. The Chef development kit is installed to /opt/chefdk/ on UNIX and Linux systems. 
After installation is finished, open command prompt and run following command

    chef verify
    
This command will run verification for 'berkshelf', 'test-kitchen', 'chef-dk', 'chef-provisioning',  'chefspec', 'openssl' etc. Once the installation is finished properly, above command should pass successfully for all components.

This [link](https://docs.chef.io/install_dk.html#uninstall-the-chef-dk-title) gives a good description of installing and uninstallting Chef Development Kit.


##### 3. Download chef-repo

You can either install git and clone chef-repo from [this](https://github.com/chef/chef-repo) location or you can directly click on [download zip](https://github.com/chef/chef-repo/archive/master.zip) and extract it to any directory.

##### 4. Configure chef-repo
Once the above downloaded package is extracted (I have extracted it in C drive so my folder structure look like this **C:/chef-repo**










