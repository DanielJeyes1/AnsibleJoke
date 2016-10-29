# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
	#Gen VM config
	config.vm.box = "geerlingguy/centos7"
	config.ssh.insert_key = false
	config.vm.synced_folder ".", "/vagrant", disabled: true
	config.vm.provider :virtualbox do |v|
		v.memory = 1024
		v.linked_clone = true
	end

# App Server 1.
	config.vm.define "app1" do |app|
		app.vm.hostname = "orc-app1.dev"
		app.vm.network :private_network, ip: "192.168.60.4"
	end
# App Server 2.
	config.vm.define "app2" do |app|
		app.vm.hostname = "orc-app2.dev"
		app.vm.network :private_network, ip: "192.168.60.5"
	end

# App Server 3.
	config.vm.define "app3" do |app|
		app.vm.hostname = "orc-app3.dev"
		app.vm.network :private_network, ip: "192.168.60.6"
	end

# App Server 4.
	config.vm.define "app4" do |app|
		app.vm.hostname = "orc-app4.dev"
		app.vm.network :private_network, ip: "192.168.60.7"
	end

# App Server 5.
	config.vm.define "app5" do |app|
		app.vm.hostname = "orc-app5.dev"
		app.vm.network :private_network, ip: "192.168.60.8"
	end			
# DB Server 1.
	config.vm.define "db" do |db|
		db.vm.hostname = "orc-db1.dev"
		db.vm.network :private_network, ip: "192.168.60.9"
	end

# DB Server 2.
	config.vm.define "db2" do |db|
		db.vm.hostname = "orc-db2.dev"
		db.vm.network :private_network, ip: "192.168.60.10"
	end

# DB Server 3.
	config.vm.define "db3" do |db|
		db.vm.hostname = "orc-db3.dev"
		db.vm.network :private_network, ip: "192.168.60.11"
	end

# DB Server 4.
	config.vm.define "db4" do |db|
		db.vm.hostname = "orc-db4.dev"
		db.vm.network :private_network, ip: "192.168.60.12"
	end

end
