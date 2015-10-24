# -*- mode ruby -*-
Vagrant.configure(2) do |config|
  config.vm.box = "box-cutter/fedora22"
  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--memory", "1024"]
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yaml"
    ansible.inventory_path = "ansible/hosts"
    ansible.limit = 'all'
    ansible.verbose = "v"
  end
end
