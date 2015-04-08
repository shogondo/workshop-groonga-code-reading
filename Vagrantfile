Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu-14.04_amd64"
  config.ssh.forward_agent = true
  config.vm.provider "virtualbox" do |vbox|
    vbox.name = "groonga-code-reading-workshop"
    vbox.customize ["modifyvm", :id, "--memory", "1024", "--cpus", "1", "--ioapic", "on"]
    vbox.customize ["modifyvm", :id, "--natdnsproxy1", "off"]
    vbox.customize ["modifyvm", :id, "--natdnshostresolver1", "off"]
  end
end
