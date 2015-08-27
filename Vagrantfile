Vagrant.configure(2) do |config|
  config.vm.box = "debian/jessie64"
  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
  end
  config.vm.provision :shell, path: "nginx.sh"
end
