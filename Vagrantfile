Vagrant.configure(2) do |config|
	config.vm.define "devops-box" do |devbox|
		devbox.vm.box = "ubuntu/bionic64"
    		devbox.vm.network "private_network", ip: "192.168.205.20"
    		devbox.vm.hostname = "devops-box"
      		devbox.vm.provision "shell", path: "scripts/install.sh"
    		devbox.vm.provider "virtualbox" do |v|
    		  v.memory = 2048
    		  v.cpus = 2
    		end
	end
end
