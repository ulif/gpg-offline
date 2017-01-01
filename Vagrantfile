# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  # If true, then any SSH connections made will enable agent forwarding.
  config.ssh.forward_agent = true

  config.vm.define "debian", primary: true do |sub|
    sub.vm.box = "debian/jessie64"
    sub.vm.provision "ansible" do |ansible|
      ansible.verbose = "v"
      ansible.playbook = "provision.yml"
    end
  end

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
  end

end
