# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  
    config.vm.define "web" do |web|
     web.vm.box = "ubuntu/bionic64"
     web.vm.network "forwarded_port", guest: 80, host: 8080
     web.vm.network "private_network", ip: "192.168.56.10"
    end
  
    config.vm.define "db" do |db|
     db.vm.box = "ubuntu/bionic64"
     db.vm.network "private_network", ip: "192.168.56.11"
    end 
  
  end