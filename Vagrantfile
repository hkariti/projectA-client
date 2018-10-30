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
  # boxes at https://atlas.hashicorp.com/search.
  config.vm.network "private_network", type: "dhcp"
  config.vm.define "default" do |bionic|
      bionic.vm.box = "ubuntu/bionic64"
      bionic.vm.provision "shell", path: "bootstrap.sh"
  end

  config.vm.define "xenial" do |xenial|
      xenial.vm.box = "ubuntu/xenial64"
  end
end
