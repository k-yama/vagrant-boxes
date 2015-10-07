# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "CentOS-6.7-minimal-ja"
  config.vm.hostname = "localhost"
  config.vm.network :forwarded_port, guest: 443, host: 8443
  config.vm.network :forwarded_port, guest: 5432, host: 15432
  config.vm.network :private_network, ip:"192.168.33.199"
  config.vm.synced_folder ".", "/var/tmp/www", :mount_options => ["dmode=777,fmode=666"]

end

