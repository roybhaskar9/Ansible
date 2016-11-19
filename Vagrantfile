Vagrant.configure(2) do |config|

 config.vm.define "acs" do |acs|
   acs.vm.box = "centos/7"
   acs.vm.hostname = "acs"
   acs.vm.network "private_network",ip:"192.168.33.10"
   config.vm.synced_folder ".","/vagrant",disabled:true
 end

 config.vm.define "web" do |web|
   web.vm.box = "centos/7"
   web.vm.hostname = "web"
   web.vm.network "private_network",ip:"192.168.33.20"
   web.vm.network "forwarded_port",guest:80,host:8080
   config.vm.synced_folder ".","/vagrant",disabled:true
 end

 config.vm.define "db" do |db|
   db.vm.box = "centos/7"
   db.vm.hostname = "db"
   db.vm.network "private_network",ip:"192.168.33.30"
   config.vm.synced_folder ".","/vagrant",disabled:true
 end
end
