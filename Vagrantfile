Vagrant.configure("2") do |config|
  config.vm.box = "generic/alpine317"
  config.vm.synced_folder ".", "/vagrant"

  config.vm.provision "shell", inline: <<-SHELL
    apk add libc6-compat nano git gcc musl-dev
  SHELL
end