Vagrant.configure(2) do |config|

 config.vm.define "acs" do |acs|
   acs.vm.box = "ubuntu/xenial64"
   acs.vm.hostname = "acs"
   acs.vm.network "private_network",ip:"192.168.33.10"
 end

 config.vm.define "web" do |web|
   web.vm.box = "ubuntu/xenial64"
   web.vm.hostname = "web"
   web.vm.network "private_network",ip:"192.168.33.20"
 end

 config.vm.define "db" do |db|
   db.vm.box = "ubuntu/xenial64"
   db.vm.hostname = "db"
   db.vm.network "private_network",ip:"192.168.33.30"
 end
end
