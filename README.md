# Requirements

You need to install the following tools to execute this sample

* [Ansible 1.4](http://www.ansibleworks.com/docs/intro_getting_started.html)

# Setup

```
$ git clone https://github.com/nulab/ansible-sample.git
$ cd ansible-sample
```


# Run modules

To run shell example on local hosts, run the following command.
```
$ ansible -m clipboard -i hosts local -a "message='hello ansible module'"
```
