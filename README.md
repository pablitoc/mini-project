# Mini Project

This is a project that provisions a webserver to serve a static HTML page.  It leverages Ansible to deploy an EC2 instance and installs all necessary resoruces to display a static nginx page.

### Installation
1. If you do not have Ansible installed already you can follow the steps provided below:

   - [For OSX](http://docs.ansible.com/ansible/intro_installation.html#latest-releases-on-mac-osx)
   - [For Ubuntu](http://docs.ansible.com/ansible/intro_installation.html#latest-releases-via-apt-ubuntu)
   - [Other](http://docs.ansible.com/ansible/intro_installation.html)

2. Unencrypt the private ssh key and add it to your keychain using the following commands:
   - `printf "ENTER PASSWORD EMAILED" > ansible_vault.txt`
   - `ansible-vault decrypt stilligent_rsa`
   - `ssh-add  stilligent_rsa`

### Running the playbook

After installing Ansible and its dependencies you can run the following command:

`ansible-playbook provision.yml`