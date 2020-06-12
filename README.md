# kali-packer-vagrant-vmware

## Setup and Config

assumes a local environment which includes `vmware fusion pro` 11 and the [vagrant vmware provider plugin](https://www.vagrantup.com/vmware#buy-now).

uses `kali-2019.4/kali-linux-2019.4-gnome-amd64` image of kali linux.

`packer` uses `kali.json` and `preseed.cfg` to configure the installation process & `scripts/setup.sh` for post-intallation configuration.

`vagrant` uses `ansible` and `playbook.yml` to configure the VM after the packer build.

## Use

run `./run-packer.sh` to build a `Kali.box` file to use with `vagrant` and `vmware fusion`. 

run `./run-vagrant.sh` to run `Kali.box`. 
