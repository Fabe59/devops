Vagrant.configure("2") do |config|

  config.vm.define "dev" do |subconfig|
  	subconfig.vm.box = "ubuntu/xenial64"
	subconfig.vm.hostname ="dev"
  	subconfig.vm.network "private_network", ip: "192.168.33.10"
  	subconfig.vm.provider "virtualbox" do |vb|
      		vb.memory = "2048"
      		vb.cpus = "1"
	end
  end

  config.vm.define "ansible" do |subconfig|
        subconfig.vm.box = "ubuntu/xenial64"
	subconfig.vm.hostname ="ansible"
        subconfig.vm.network "private_network", ip: "192.168.33.20"
        subconfig.vm.provider "virtualbox" do |vb|
                vb.memory = "2048"
                vb.cpus = "2"
        end
  end

  config.vm.define "jenkins" do |subconfig|
        subconfig.vm.box = "ubuntu/xenial64"
        subconfig.vm.hostname ="jenkins"
        subconfig.vm.network "private_network", ip: "192.168.33.30"
        subconfig.vm.provider "virtualbox" do |vb|
                vb.memory = "6000"
                vb.cpus = "2"
        end
  end

  config.vm.define "serveur" do |subconfig|
        subconfig.vm.box = "ubuntu/xenial64"
        subconfig.vm.hostname ="serveur"
        subconfig.vm.network "private_network", ip: "192.168.33.40"
        subconfig.vm.provider "virtualbox" do |vb|
                vb.memory = "4000"
                vb.cpus = "2"
        end
  end

    config.vm.define "monitoring-server" do |subconfig|
        subconfig.vm.box = "ubuntu/xenial64"
        subconfig.vm.hostname ="monitoring-server"
        subconfig.vm.network "private_network", ip: "192.168.33.50"
        subconfig.vm.provider "virtualbox" do |vb|
                vb.memory = "8000"
                vb.cpus = "2"
        end
  end

end
