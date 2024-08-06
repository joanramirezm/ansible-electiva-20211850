Vagrant.configure("2") do |config|
    (1..3).each do |num|
      config.vm.define "node#{num}" do |node|
        node.vm.box = "ubuntu/bionic64"
        node.vm.hostname = "node#{num}"
        node.vm.network "private_network", type: "dhcp"
        node.vm.provider "virtualbox" do |vb|
          vb.memory = "256"
          vb.cpus = 1
        end
      end
    end
  end