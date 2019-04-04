# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

	config.vm.define "control" do |control|
		control.vm.box = "ubuntu/trusty64"
		control.vm.hostname = "control"
		control.vm.network "private_network", ip: "192.168.33.40"
		control.vm.synced_folder "./control", "/home/vagrant/test", type:"virtualbox"
	end

	config.vm.define "webserver" do |webserver|
		webserver.vm.box = "ubuntu/trusty64"
		webserver.vm.hostname = "webserver"
		webserver.vm.network "private_network", ip: "192.168.33.50"
	end

	config.vm.define "database" do |database|
		database.vm.box = "ubuntu/trusty64"
		database.vm.hostname = "database"
		database.vm.network "private_network", ip: "192.168.33.60"
	end

	config.vm.define "tensor" do |tensor|
		tensor.vm.box = "ubuntu/trusty64"
		tensor.vm.hostname = "tensor"
		tensor.vm.network "private_network", ip: "192.168.33.70"
	end

	
end