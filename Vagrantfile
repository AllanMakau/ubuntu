$script_teste = <<-SCRIPT
	touch teste.txt
SCRIPT


Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/bionic64"
  config.vm.hostname = "ubuntulab"

  config.vm.provider "virtualbox" do |v|
   v.name = "ubuntu"
   v.memory = 1024
   v.cpus = 2
  end

  config.vm.provision "shell", inline:  $script_teste
  	
end

