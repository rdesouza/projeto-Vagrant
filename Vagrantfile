Vagrant.configure("2") do |config|
config.vm.box = "ubuntu/focal64"

  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.network "public_network"

  config.vm.synced_folder "../vagrant", "/var/www/html"

  config.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.name = "projeto-vagrant"
  end

  config.vm.provision "shell", inline: <<-SHELL
      apt-get update
      apt-get install -y nginx
    SHELL
end
