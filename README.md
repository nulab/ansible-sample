# Requirements

You need to install the following tools to execute this sample.

* [Vagrant 1.3](http://docs.vagrantup.com/v2/installation/index.html)
* [Ansible 1.4](http://www.ansibleworks.com/docs/intro_getting_started.html)

# Setup

```
$ git clone https://github.com/nulab/ansible-sample.git
$ cd ansible-sample
$ vagrant up
$ vagrant ssh-config > ssh.config
```

# Run sample modules

Running a bash module on localhost is like this.

```
$ ansible -m clipboard -i hosts local -a "message='hello ansible module'"
```

Running a python module on vagrant host is like this. You may have to change the value of ANSIBLE_REMOTE_PORT according to your vagrant environment. Check your "Port" value described in ssh.config.

```
$  ANSIBLE_REMOTE_PORT=2222 ANSIBLE_SSH_ARGS="-F ssh.config" ansible default -i hosts -m serf -s -a "version=0.3.0"
```

