# Requirements

You need to install the following tools to execute this sample

* [Ansible 1.4](http://www.ansibleworks.com/docs/intro_getting_started.html)

# Setup

```
$ git clone https://github.com/nulab/ansible-sample.git
$ cd ansible-sample
```


# Run sample modules

Running a bash module on local hosts is like this.
```
$ ansible -m clipboard -i hosts local -a "message='hello ansible module'"
```
