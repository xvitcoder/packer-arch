# packer-arch

### Create virtualbox image
```
packer build -only=virtualbox-iso arch-template.json
```
### Add the new box to vagrant
```
vagrant box add arch output/packer_arch_virtualbox.box
```

### Vagrantfile
```
# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "arch"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "4096"
    vb.cpus = 2
  end
end
```
