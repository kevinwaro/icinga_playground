# -*- mode: ruby -*-
Vagrant.configure(2) do |config|
 config.vm.define "icinga2" do |icinga2|
   icinga2.vm.box ="debian/bullseye64" 
   icinga2.vm.network "private_network", ip: "192.168.200.10"
   icinga2.vm.hostname = "icinga2"
   icinga2.vm.provider "virtualbox" do |vb|
     vb.memory = "2048"
     vb.cpus = 2
   end
   icinga2.vm.provision "ansible/icinga2", type: "ansible" do |ansible|
     ansible.playbook = "icinga2.yml"
     ansible.verbose = "v"
     ansible.extra_vars = {
       "target" => "icinga2",
       }
   end
 end

end

