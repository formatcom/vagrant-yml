# -*- mode: ruby -*-
# vi: set ft=ruby :

require 'yaml'

VAGRANTFILE_API_VERSION = "2"

# load config yaml
vm = {}
vm['config'] = YAML.load_file('config.vm.yml')

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

	# config virtual machine
	vm['config']['machines'].each do |machine|

		config.vm.define machine['name'] do |node|

			node.vm.box = machine['box']
			node.vm.network :private_network, :ip => machine['ip']
			node.vm.provision :hosts, :sync_hosts => true

		end
	end

end

