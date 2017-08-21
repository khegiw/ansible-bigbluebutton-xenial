# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://vagrantcloud.com/search.
  config.vm.box = "ubuntu/xenial64"
#   config.vm.network "public_network"
# config.vm.provider "virtualbox" do |v|
#         v.memory = 4100
#         v.cpus = 2
#     end
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.network "forwarded_port", guest: 443, host: 4430
  config.vm.network "forwarded_port", guest: 1935, host: 19350
  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y ansible
  #   cd /vagrant && sudo ansible-playbook test.yml
  # SHELL
  # config.vm.provision "shell", inline: <<-SHELL
  #   cd /vagrant && sudo ansible-playbook test.yml
  # SHELL

end
