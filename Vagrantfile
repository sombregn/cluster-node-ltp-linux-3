Vagrant.configure("2") do |config|

  # Machine Web
  config.vm.define "web" do |web|
    web.vm.box = "bento/ubuntu-22.04"
    web.vm.box_check_update = false
    web.vm.network "forwarded_port", guest: 8086, host: 8086
    web.vm.network "private_network", ip: "192.168.56.10"
    web.vm.synced_folder "./web", "/var/www/html"

    web.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.cpus = 1
      vb.name = "web"
      vb.memory = "1024"
    end
  end

  # Machine DB
  config.vm.define "db" do |db|
    db.vm.box = "bento/ubuntu-22.04"
    db.vm.box_check_update = false
    db.vm.network "private_network", ip: "192.168.56.11"
    db.vm.hostname = "db"

    db.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.memory = "1024"
      vb.cpus = 1
      vb.name = "db"
    end
  end
end