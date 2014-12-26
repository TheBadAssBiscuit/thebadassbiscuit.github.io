# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"
  #config.vm.box_url = "http://files.vagrantup.com/precise32.box"
  config.vm.network :forwarded_port, host: 4000, guest: 4000
  config.vm.provision :shell, :inline => "apt-get update && apt-get -y install build-essential ruby-dev && gem install github-pages"

end
