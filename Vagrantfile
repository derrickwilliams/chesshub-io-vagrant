VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.network "forwarded_port", guest: 28017, host: 28017
  config.vm.network "forwarded_port", guest: 27017, host: 27017

  config.vm.provision 'shell', path: 'provision.sh'
end
