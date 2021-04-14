# cloud-on-cloud
- set up your own private cloud on top of the Google Cloud using OpenStack and kolla-ansible
## Requirements
- Unix based OS (i.e. Ubuntu 20.4 VM)
- Google Cloud Account
- Google Cloud SDK set up
## Usage
This is how to spin up your own private cloud
### Prepare VMs on the Google cloud
- Run `./spinup-gcp-for-openstack.sh`
### Install OpenStack
- Open the files `multinode` and `globals.yml`. Replace the placeholders “[******<>******]” with respective values
- Run `kolla-ansible/deploy-openstack.sh`
## Configure OpenStack
- Run `./prepare-openstack.sh`
- Enter the public IP address of the controller VM in your beowser to access the OpenStack login page

