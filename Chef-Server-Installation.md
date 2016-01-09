## Steps to Install Chef Server
I am using RHEL6 server for this exercise. You need to follow following steps to install chef server.  

          1. Download Chef Server 
          2. Install Chef Server
          3. Create User
          4. Create Organization

### 1. Download Chef Server
#####i. Install wget on your server
          sudo yum install wget -y

#####ii. Choose appropriate version
Go to the [download link](https://downloads.chef.io/chef-server/), choose the Operating System and version of chef server you want to use.

#####iii. Download Chef Server
          wget https://packagecloud.io/chef/stable/packages/el/6/chef-server-core-12.3.1-1.el6.x86_64.rpm/download
          (this will download chef server 12.3.1 for RHEL 6.)
          
### 2. Install Chef Server

