
Vagrant.configure("2") do |config|
  config.vm.box = "python-box"
 config.vm.provision "shell", inline:<<-SHELL
    apt-get update
    apt -y install python3.10
    apt -y install python3-pip
    apt -y install python3-psycopg2
    apt -y install python3-django
    mkdir -p /script && cp /vagrant/*.txt /script
 SHELL

end
