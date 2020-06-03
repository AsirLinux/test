# -*- mode: ruby -*-
# vi: set ft=ruby :
# We need to ensure the vagarant installed or not with oracle virtulbox
# this vagarnt file used to launch Ansible & Puppet by single play

Vagrant.configure("2") do |config|
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2	
  end

  config.vm.define "AnsibleMaster" do |pm|
    pm.vm.box = "centos/7"
    pm.vm.network "private_network", ip: "192.168.33.10"
    pm.vm.hostname = "AnsibleMaster"
  end

  config.vm.define "AnsibleCentos7" do |pac|
    pac.vm.box = "centos/7"
    pac.vm.network "private_network", ip: "192.168.33.11"
    pac.vm.hostname = "AnsibleCentos7"
  end

  config.vm.define "AnsibleCentos6" do |pac|
    pac.vm.box = "centos/6"
    pac.vm.network "private_network", ip: "192.168.33.12"
    pac.vm.hostname = "AnsibleCentos6"
  end

  config.vm.define "PuppetMaster" do |pm|
    pm.vm.box = "centos/7"
    pm.vm.network "private_network", ip: "192.168.33.20"
    pm.vm.hostname = "PuppetMaster"
  end

  config.vm.define "PuppetCentos7" do |pac|
    pac.vm.box = "centos/7"
    pac.vm.network "private_network", ip: "192.168.33.21"
    pac.vm.hostname = "PuppetCentos7"
  end  

  config.vm.define "PuppetCentos6" do |pac|
    pac.vm.box = "centos/6"
    pac.vm.network "private_network", ip: "192.168.33.22"
    pac.vm.hostname = "PuppetCentos6"
  end
end
