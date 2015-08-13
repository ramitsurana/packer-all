# Packer-all

This is a packer image that works on Openstack,AWS,VMWare,Azure etc.

## Instructions

1.  Install http://packer.io according to directions.
2.  Clone this repository.
3.  Modify some basic settings.
4.  To create a VMWare Fusion machine run the command `packer build vmware-example.json`
5.  To create an Amazon AMI run the command `packer build ami-example.json`
6.  To create both at the same time, run `packer build system-build.json`.
