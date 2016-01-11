## Steps to Install Chef Server
I am using RHEL6 server for this exercise. You need to follow following steps to install chef server.  

          1. Download Chef Server 
          2. Install Chef Server
          3. Create User
          4. Create Organization

### 1. Download Chef Server
#####i. Install wget on your server

For RHEL server, execute

          sudo yum install wget -y 
          
For Ubuntu server, execute

          sudo apt-get install wget

#####ii. Choose appropriate chef server version
Go to the [download link](https://downloads.chef.io/chef-server/), choose the Operating System and version of chef server you want to use.

#####iii. Download Chef Server
          wget https://packagecloud.io/chef/stable/packages/el/6/chef-server-core-12.3.1-1.el6.x86_64.rpm/download
(this will download chef server 12.3.1 for RHEL 6.)
          
          
### 2. Install Chef Server
This activity needs root access. If  you are not executing this command from the directory where your chef package recides then you will have to specify full path.
For RedHat:

          sudo rpm -Uvh chef-server-core-12.3.1-1.el5.x86_64.rpm

For Ubuntu:
This will install chef server. It typically takes less than a min.

          dpkg -i chef-server-core-12.3.1-1.el5.x86_64.deb
          

This will start all required services. It typically takes around 5 mins to finish.

          chef-server-ctl reconfigure
At this state your Chef server is installed and functional. You can check "http://IP_of_chef_server". It should give you chef server home page.

### 3. Create User
Following command will create administrator user for chef and generate admin.pem file.

          chef-server-ctl user-create *USERNAME FIRST_NAME LAST_NAME EMAIL PASSWORD*
          
          USERNAME = 
          FIRST_NAME = 
          LAST_NAME =
          EMAIL = 
          PASSWORD = 
          
Example:

          

