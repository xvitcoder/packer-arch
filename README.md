# packer-arch

### Create virtualbox image
```
git clone https://github.com/elasticdog/packer-arch.git
cd packer-arch/
packer build -only=virtualbox-iso arch-template.json
```
### Add the virtualbox to vagrant
```
vagrant box add arch output/packer_arch_virtualbox.box
```
