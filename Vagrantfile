Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.synced_folder '.', '/vagrant', disabled: true
  config.vm.provider "virtualbox" do |v|
    v.memory = 512
    v.cpus = 1
  end

  # centos manage VM
  config.vm.define 'manage' do |manage|
    manage.vm.hostname = 'manage.local'
    manage.vm.network :private_network, ip: '192.168.13.113'
  end

  # centos  node_1 VM
  config.vm.define 'node01' do |node01|
    node01.vm.hostname = 'node01.local'
    node01.vm.network :private_network, ip: '192.168.13.114'
  end

  # centos node_2 VM
  config.vm.define 'node02' do |node02|
    node02.vm.hostname = 'node02.local'
    node02.vm.network :private_network, ip: '192.168.13.115'
  end

  # Ansible
#  config.vm.provision "ansible" do |ansible|
#    ansible.playbook = "playbook.yml"
#  end
end
