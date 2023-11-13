# -*- mode: ruby -*-
# vi: set ft=ruby :

IP =  "192.168.58.108"   # Ip address
CPU_CORES_COUNT = "12"   # CPU cores
MEMORY_COUNT = "16384"   # OS Memory

Vagrant.configure("2") do |macos|
    macos.vm.box = "droy/macMonterey"
    # macos.vm.synced_folder ".", "/vagrant", disabled: true
    macos.vm.synced_folder "shared", "/home/vagrant/Shared"
    macos.vm.network :private_network, ip: IP
    macos.vm.provider "vmware_desktop" do |vb|
        vb.memory = MEMORY_COUNT
        vb.cpus = CPU_CORES_COUNT
        vb.gui = true
  end
end
