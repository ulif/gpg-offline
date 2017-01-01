# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  # If true, then any SSH connections made will enable agent forwarding.
  config.ssh.forward_agent = true

  config.vm.define "debian", primary: true do |sub|
    sub.vm.box = "debian/jessie64"
  end

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
  end

end
