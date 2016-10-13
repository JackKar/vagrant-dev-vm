# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"
   Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
       config.vm.box = "minimum/ubuntu-trusty64-docker"
       config.vm.provider :virtualbox do |vb|
           vb.customize ["modifyvm", :id, "--memory", 1024]
       end
       config.ssh.insert_key = false
    #   config.ssh.username = 'root'
    #   config.ssh.password = 'vagrant'
       config.vm.provision "shell", inline: "sudo apt-get -y install subversion"
   end