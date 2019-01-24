# Packer Syspass Build - CentOS 7 minimal Vagrant Box using Ansible provisioner

## Requirements

The following software must be installed/present on your local machine before you can use Packer to build the Vagrant box file:

  - [Packer](http://www.packer.io/)
  - [Vagrant](http://vagrantup.com/)
  - [VirtualBox](https://www.virtualbox.org/) (if you want to build the VirtualBox box)
  - [Ansible](http://docs.ansible.com/intro_installation.html)

## Usage

Make sure all the required software (listed above) is installed, then cd to the directory containing this README.md file, and run:

    $ packer build centos7.json

After a few minutes, Packer should tell you the box was generated successfully.


## Run sysPass docker-compose file

There's an included Vagrantfile that allows to provision sysPass app and db containers, in order to be used restoring a sysPass instance. Cd to the directory containing this README.md file, and run:

    $ vagrant up

After a few minutes, sysPass will accept connections to the private IP defined in Vagrantfile.
