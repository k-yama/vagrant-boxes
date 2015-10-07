# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "CentOS-6.7-minimal-ja"
  config.vm.box_url = "https://github.com/yamakuda/vagrant-boxes/releases/download/1.0.0/CentOS-6.7-minimal-ja.box"

  config.vm.hostname = "localhost"

  config.vm.network :forwarded_port, guest: 5432, host: 15432 # PostgreSQL
  config.vm.network :forwarded_port, guest: 3306, host: 13306 # MySQL

  config.vm.network :private_network, ip:"192.168.33.199"
  config.vm.synced_folder ".", "/var/tmp/www", :mount_options => ["dmode=777,fmode=666"]

end

