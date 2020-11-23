# First Virtual Box, Vagrant Dev Environment

This repo is our first Virtual Environment to create a Dev Environment

## Virtual Box
What is it?



## Vagrant
What is it?

Vagrant boxes - Pre leaded vagrant files that create virtual machines. Usually just an OS.

Ubunto is an open source OS
Ubuntu with GUI (Graphical user interface) - Looks like a desktop and works like one
Ubuntu headless - is basically a terminal, no GUI. (this is the one we will use).
  - Faster
  - More secure
  - Lighter

### Main commands

- `vagrant init`
  - Makes vagrant file in repo
- `vagrant init <box>`
  - can search for boxes in https://app.vagrantup.com/<box> and it installs that box
- `vagrant up`
  - creates virtual environment
- `vagrant destroy`
  - destroys virtual environment
##### Task 1
- Vagrant up with ubuntu/xenial64
- vagrant destroy
- delete your vagrant file
- use vagrant init to create vagrant file with centos 7
- vagrant up again
- vagrant destroy

**Take notes of machines being created in virtual box**

##### Task 2
- create a vagrant box with ubuntu version 18.04
- Find the command to SSH into the machine
- Create a README.md file inside machine and write your name and your favourite movie

###### Solution
- `vagrant init`
- change vagrant file to 
```
Vagrant.configure("2") do |config|
config.vm.box = "ubuntu/xenial64"
end
```
- `vagrant up`
- `vagrant ssh`
![](img/vagrant_ssh.png)
- linux commands to make readme `nano README.md`
- `exit`
![](img/exit_virtual_machine.png)
