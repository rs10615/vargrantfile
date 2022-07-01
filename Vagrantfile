Vagrant.configure("2") do |config|
 
config.vm.define :web1 do |web1_config|
  web1_config.vm.box = "centos/7"
  web1_config.vm.box_url = "https://app.vagrantup.com/centos/boxes/7"

 
   web1_config.vm.box_check_update = false
 
 
   web1_config.vm.network "private_network", ip: "10.170.1.14"
   #web1_config.vm.network "public_network"
   web1_config.vm.network "forwarded_port", guest: 22, host: 3204 ,id: "ssh" , auto_correct: true   

   web1_config.vm.hostname = "web1admin"  # ensure you have local write access to C:/windows/system32/drivers/etc/host "
#   web1_config.vm.synced_folder "D:\\TOOLS", "/tools"
 

 
end
config.vm.define :web2 do |web2_config|
  web2_config.vm.box = "bento/ubuntu-18.04"
  web2_config.vm.box_url = "https://app.vagrantup.com/bento/boxes/ubuntu-18.04"

 
   web2_config.vm.box_check_update = false
 
 
   web2_config.vm.network "private_network", ip: "10.170.1.14"
   #web2_config.vm.network "public_network"
   web2_config.vm.network "forwarded_port", guest: 22, host: 3204 ,id: "ssh" , auto_correct: true
   

   web2_config.vm.hostname = "web1admin"  # ensure you have local write access to C:/windows/system32/drivers/etc/host "
#   web2_config.vm.synced_folder "D:\\TOOLS", "/tools"
 

 
end 
config.vm.define :red do |red_config|
  red_config.vm.box = "williamyeh/centos7-docker"
  red_config.vm.box_url = "https://app.vagrantup.com/williamyeh/boxes/centos7-docker"

 
   red_config.vm.box_check_update = false
 
 
   red_config.vm.network "private_network", ip: "10.170.1.14"
   #red_config.vm.network "public_network"
   red_config.vm.network "forwarded_port", guest: 22, host: 3204 ,id: "ssh" , auto_correct: true
   red_config.vm.network "forwarded_port", guest: 8080, host: 18000
   red_config.vm.network "forwarded_port", guest: 16686, host: 16686
   red_config.vm.network "forwarded_port", guest: 14267, host: 14267
   red_config.vm.network "forwarded_port", guest: 14268, host: 14268
   red_config.vm.network "forwarded_port", guest: 5775	, host: 5775, protocol: "udp"	
   red_config.vm.network "forwarded_port", guest: 6831, host: 6831, protocol: "udp"
   red_config.vm.network "forwarded_port", guest: 6832, host: 6832, protocol: "udp"
   red_config.vm.network "forwarded_port", guest: 5778, host: 5778
   red_config.vm.network "forwarded_port", guest: 9411, host: 9411
   red_config.vm.network "forwarded_port", guest: 2181, host: 2181
   red_config.vm.network "forwarded_port", guest: 9092, host: 9092
   red_config.vm.network "forwarded_port", guest: 8500, host: 8500
   red_config.vm.network "forwarded_port", guest: 8443, host: 8443
   red_config.vm.network "forwarded_port", guest: 9443, host: 9443
   red_config.vm.network "forwarded_port", guest: 12000, host: 12000
   red_config.vm.network "forwarded_port", guest: 6379, host: 6379
   red_config.vm.network "forwarded_port", guest: 9099, host: 9099
   red_config.vm.network "forwarded_port", guest: 8765, host: 8765
   red_config.vm.network "forwarded_port", guest: 8091, host: 8091
   red_config.vm.network "forwarded_port", guest: 8092, host: 8092
   red_config.vm.network "forwarded_port", guest: 8093, host: 8093
  red_config.vm.network "forwarded_port", guest: 8094, host: 8094
  red_config.vm.network "forwarded_port", guest: 9876, host: 9876
  red_config.vm.network "forwarded_port", guest: 9877, host: 9877
   red_config.vm.network "forwarded_port", guest: 8081, host: 8081

  
  #red_config.vm.network "forwarded_port", guest: 9098, host: 9098




   red_config.vm.hostname = "redadmin"  # ensure you have local write access to C:/windows/system32/drivers/etc/host "
#   red_config.vm.synced_folder "D:\\TOOLS", "/tools"
 
end
 
config.vm.define :red2 do |red2_config|
  red2_config.vm.box = "williamyeh/centos7-docker"
  red2_config.vm.box_url = "https://app.vagrantup.com/williamyeh/boxes/centos7-docker"

 
   red2_config.vm.box_check_update = false
 
 
   red2_config.vm.network "private_network", ip: "10.170.1.14"
   #red2_config.vm.network "public_network"
   red2_config.vm.network "forwarded_port", guest: 22, host: 3204 ,id: "ssh" , auto_correct: true
  red2_config.vm.network "forwarded_port", guest: 9876, host: 9877
  



   red2_config.vm.hostname = "red2admin"  # ensure you have local write access to C:/windows/system32/drivers/etc/host "
#   red2_config.vm.synced_folder "D:\\TOOLS", "/tools"
 
end
 
end