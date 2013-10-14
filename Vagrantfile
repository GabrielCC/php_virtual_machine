Vagrant::Config.run do |config|
	config.vm.box       = 'precise32'
	config.vm.box_url   = 'http://files.vagrantup.com/precise32.box'
	config.vm.host_name  = 'php-starter-box'

	config.vm.forward_port 3000, 3000
	config.vm.forward_port 80, 80 

	config.vm.provision :shell, :path => "bin/install-extra.sh"
end