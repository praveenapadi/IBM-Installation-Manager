# IBM-Installation-Manager
### Author: PraveenaPadi
This playbook can be used to install and uninstall IBM Installation Manager.

## About IBM-Installation-Manager (IIM)
IBMs Installation Manager is a tool that you can use to install and maintain your IBM software packages. Installation Manager is bundled with many IBM software products and provides the core installation capability. 

## About the playbook
The playbook was tested on CentOS. Please note that this playbook can be used to install and uninstall IIM and you can consider improving it as you move on.
This playbook uses the downloaded binaries of IIM. I have commented the code needed for online download of the binaries too incase you might need it.

Inventory: 
    inventory file in this playbook contains the list of servers on which you want IIM to be installed. 
    
group_vars:
    main.yml in this folder contains all the global vars which you want to use across all the servers.
    
roles:
    Created 2 roles one each for install and uninstall of IIM. 
       - iim-install
       - iim-uninstall
       
mainplay.yml:
    This is the main playbook which you need to run. Do comment the role which you dont need from this yaml file and run it.
