# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.box = 'vagrant-coreos-docker'

  config.vm.provider :vmware_fusion do |vmware, override|
    override.vm.box_url = 'http://storage.core-os.net/coreos/amd64-generic/dev-channel/coreos_production_vagrant_vmware_fusion.box'
    vmware.vmx['memsize'] = '1024'
  end

  config.vm.provider :virtualbox do |virtualbox, override|
    override.vm.box_url = 'http://storage.core-os.net/coreos/amd64-generic/dev-channel/coreos_production_vagrant.box'
  end

  config.vm.network :forwarded_port, guest: 4243, host: 4243

  config.ssh.username = 'core'

  config.vm.provision :shell, :path => 'scripts/tlsdated.service'
  config.vm.provision :shell, :path => 'scripts/docker.service'
end
