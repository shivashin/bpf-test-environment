# BPF Environment set up script

## Execution Environment

+ ansible 2.9.14
+ python 3.9.0
+ vagrant 2.2.10
+ VirtualBox 6.1.16

## Getting Started

After git clone, then run:
```
vagrant up
ansible-playbook playbooks/setup.yml
vagrant reload
```

## FAQ

### Q. Why does vagrant reload?

Linux verison upgrades Linux5.3+.

### Q. Why is Linux 5.3+ required?

Otherwise the BPF program will be rejected due to the maximum instruction limit (see [this commit](https://github.com/torvalds/linux/commit/c04c0d2b968ac45d6ef020316808ef6c82325a82).)
