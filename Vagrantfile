# -*- mode: ruby -*-
# vi: set ft=ruby :
# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
require 'yaml'
secmachines = YAML.load_file("machines.yml")

Vagrant.configure("2") do |config|
	secmachines.each do |machines|
		config.vm.define machines["name"] do |server|
			server.vm.hostname = machines["name"]
			server.vm.box = machines["so"]
			server.vm.network "private_network", ip: machines["ip"], dns: "8.8.8.8" 

			server.vm.provider "virtualbox" do |vb|
				vb.memory = machines["memory"]
				vb.cpus = machines["cpus"]
			end
		end
		
  	config.vm.provision "shell", inline: <<-SHELL
  	  mkdir -p /root/.ssh/
  	  cat /vagrant/infraagil.pem > /root/.ssh/id_rsa
  	  cat /vagrant/infraagil.pub > /root/.ssh/authorized_keys
  	  chmod 600 /root/.ssh/id_rsa
  	SHELL
	end
end
