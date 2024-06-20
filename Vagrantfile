Vagrant.configure("2") do |config|
    config.vm.box = "generic/ubuntu2204"

    config.vm.define 'ubuntu-2204'

    config.vm.provider "virtualbox" do |vb|
      # Customize the amount of memory on the VM:
      vb.memory = "1024"
      vb.cpus=1
    end

    # Prevent SharedFoldersEnableSymlinksCreate errors
    config.vm.synced_folder ".", "/vagrant", disabled: true
end