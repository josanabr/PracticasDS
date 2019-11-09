# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.define "rpc01" do |web|
        web.vm.network "private_network", ip: "192.168.200.53"
        web.vm.provision "shell", path: "rpc.sh"
  	web.vm.provider :virtualbox do |vb|
		vb.customize [ 'modifyvm', :id, '--memory', '386' ]
		vb.customize [ 'modifyvm', :id, '--cpus', '1' ]
		vb.customize [ 'modifyvm', :id, '--name', 'rpc01' ]
  	end
  end
  config.vm.define "rpc02" do |web|
        web.vm.network "private_network", ip: "192.168.200.54"
        web.vm.provision "shell", path: "rpc.sh"
  	web.vm.provider :virtualbox do |vb|
		vb.customize [ 'modifyvm', :id, '--memory', '386' ]
		vb.customize [ 'modifyvm', :id, '--cpus', '1' ]
		vb.customize [ 'modifyvm', :id, '--name', 'rpc02' ]
  	end
  end
end
