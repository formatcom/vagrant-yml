##REQS
~~~
- VirtualBox
- VirtualBox-webservice
- vagrant
~~~

##PLUGIN VAGRANT
~~~
- vagrant-hosts      https://github.com/oscar-stack/vagrant-hosts
- vagrant-vbguest    https://github.com/dotless-de/vagrant-vbguest
~~~

##USE
~~~
vagrant up --provider virtualbox
vagrant ssh vm1
$ ping vm2
$ exit
vagrant ssh vm2
$ ping vm1
$ exit
vagrant destroy
~~~
