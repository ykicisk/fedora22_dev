Vagrant.configure(2) do |config|
  config.vm.box = "fedora22"
  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yaml"
    ansible.inventory_path = "ansible/hosts"
    ansible.limit = 'all'
    ansible.verbose = "v"
  end
end
