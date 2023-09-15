# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.network "forwarded_port", guest: 80, host: 2000, host_ip: "127.0.0.1", guest_ip: "10.0.2.15"
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yaml"
  end
end

