## Introduction

Packer is an open source tool for creating identical machine images for multiple platforms from a single source configuration.

As the name suggests, it packages up software with complex requirements for multiple platforms in parallel. It can create consistent images across and is perfect for creating appliances and disposable product demos.

## What are we trying to do?

We want packer to create identical machine images across almsot every platform. 

To start with. we will cover the following platforms:

  - Amazon EC2 (AMI)
  - OpenStack
  - VMware (VMX)
  - Docker

Provisioning will be done by Chef.


## Expected Output

Identical machine images across platforms, with CentOs 6.x running on them. Git, Java 7.x and other basic stuff installed via Chef community cookbooks. 


## Instructions

  - Install [packer](http://packer.io) according to directions.
  - Clone the repo: `git clone https://github.com/ramitsurana/packer-all.git`
  - Modify some basic settings as required.
  - Create idential machine images by single command: `packer build system-build.json`.

At the same time, packer gives you flexibility to create images for individual platforms. For e.g:
  - Create a VMWare Fusion machine:`packer build vmware-example.json`

## Get Involved

Follow [these](https://guides.github.com/activities/contributing-to-open-source/) guidelines.

##License

  The work done has been licensed under Apache License 2.0.The license file can be found
  [here](https://github.com/ramitsurana/packer-all/blob/master/LICENSE).
  You can find out more about license,at
  
    http://www.apache.org/licenses/LICENSE-2.0
