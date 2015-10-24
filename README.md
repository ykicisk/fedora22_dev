# fedora22_dev
vagrant and ansible files for fedora22

## preparation

```bash
$ vagrant box add fedora22 https://download.fedoraproject.org/pub/fedora/linux/releases/22/Cloud/x86_64/Images/Fedora-Cloud-Base-Vagrant-22-20150521.x86_64.vagrant-virtualbox.box
$ vagrant init fedora22
```

## provision

```bash
$ vagrant up
```

if vagrant is already up, 
```bash
$ vagrant provision
```
