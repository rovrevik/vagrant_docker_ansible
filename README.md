Vagrant
=======
https://docs.vagrantup.com/v2/docker/basics.html

It is goofy but apparently you have to execute vagrant with the --provider=docker argument.

Add the inital docker config.vm.provider that uses the ubunu image.

Vagrant Docker Provisioning
===========================
https://docs.vagrantup.com/v2/provisioning/docker.html

Vagrant Docker Provider
=======================
https://docs.vagrantup.com/v2/docker/index.html

https://www.vagrantup.com/blog/feature-preview-vagrant-1-6-docker-dev-environments.html

Set up vagrant to use a different host box for all of the Docker containers.
We want to do this so that more effecient directory sharing from VirtualBox -> Docker host VM -> Docker container.

Slow network intensive bits
===========================
- Dowloading the Vagrant box? (only the first time the vagrant box needs to be downloaded)
- Importing base box 'phusion/ubuntu-14.04-amd64'... (show a percentage but doesn't take too long)
- Installing Docker (latest) onto machine... (painful)
- Pulling repository phusion/baseimage
- Right after "Pulling repository phusion/baseimage" it works for a painful long time,

TODO
====
- Add a ssh password.
- Make ssh keys work.
- Add virtualbox logging to debug slow bits.
- Add Docker logging to debug slow bits.
- Add support for not checking box and image versions.