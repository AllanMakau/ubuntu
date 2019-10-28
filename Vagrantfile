


Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/bionic64"
  config.vm.hostname = "ubuntulab"

  config.vm.provider "virtualbox" do |v|
   v.name = "ubuntu"
   v.memory = 1024
   v.cpus = 2
  end
  

  config.vm.provision :ansible_local do |ansible|
    ansible.install_mode = "default"
    ansible.playbook = "playbook.yml"
    ansible.verbose  = true
    ansible.install  = true
    ansible.limit    = "all"
  end

  	
end

