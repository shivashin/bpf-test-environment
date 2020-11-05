Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-18.04"

  config.vm.define "bpf-test" do |server|
    server.vm.network "private_network", ip: "192.168.33.10"
    server.vm.hostname = "bpf-test"
  end
end
