# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
	config.vm.define "ans" do |ans|
		ans.vm.box = "nrel/CentOS-6.7-x86_64"
		ans.vm.hostname = "ans"
		ans.vm.network "private_network", ip: "192.168.30.11"
	end
	
	config.vm.define "test1" do |test1|
		test1.vm.box = "nrel/CentOS-6.7-x86_64"
		test1.vm.hostname = "test1"
		test1.vm.network "private_network", ip: "192.168.30.21"
		test1.vm.network "forwarded_port", guest: 80, host: 80
	end
	
	config.vm.define "test2" do |test2|
		test2.vm.box = "nrel/CentOS-6.7-x86_64"
		test2.vm.hostname = "test2"
		test2.vm.network "private_network", ip: "192.168.30.22"
	end
	
	config.vm.define "test3" do |test3|
		test3.vm.box = "nrel/CentOS-6.7-x86_64"
		test3.vm.hostname = "test3"
		test3.vm.network "private_network", ip: "192.168.30.23"
	end
	
	config.vm.define "sql1" do |test3|
		test3.vm.box = "nrel/CentOS-6.7-x86_64"
		test3.vm.hostname = "sql1"
		test3.vm.network "private_network", ip: "192.168.30.31"
	end
	
end
