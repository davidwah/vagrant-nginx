Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.box_version = "20221213.0.0"
  config.vm.hostname = "node-01"
  config.vm.provision "shell", path: "provision.sh"
  config.vm.network "public_network", bridge: "wlp3s0"
  config.vm.provider :virtualbox do |vb|
    vb.memory = 1024
    vb.cpus = 1
  end
end
