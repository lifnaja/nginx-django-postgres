Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "private_network", ip: "192.168.33.33"
  config.vm.provision "shell", inline: "sudo curl -sS https://get.docker.com/ | sh"
  config.vm.provision "shell", inline: "sudo curl -L https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m) -o /usr/local/bin/docker-compose"
  config.vm.provision "shell", inline: "sudo chmod +x /usr/local/bin/docker-compose"
  config.vm.provision "file" ,source: "sample-docker", destination: "sample-docker"
  config.vm.provision "file" ,source: "compose-docker", destination: "compose-docker"
end
