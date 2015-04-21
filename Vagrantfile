# -*- mode: ruby -*-
# # vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "chef/centos-7.0"
  config.ssh.insert_key = false

  config.vm.define 'app' do |app|
    app.vm.network 'private_network', ip: '192.168.77.2'
    app.cache.scope = :box if Vagrant.has_plugin? 'vagrant-cachier'
  end
end
