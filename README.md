# packer-arch

### Create virtualbox image
```
packer build -only=virtualbox-iso arch-template.json
```
### Add the virtualbox to vagrant
```
vagrant box add arch output/packer_arch_virtualbox.box
```
