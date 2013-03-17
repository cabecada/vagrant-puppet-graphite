vagrant-puppet-graphite
=======================

Vagrant setup with a puppet module for Graphite (Metrics)

Currently module only tested to work on Ubuntu 12.04

I require the ability to create multiple instances of carbon for different teams, potentially listening on different virtual network interfaces which can then be moved onto other servers without issue.

Carbon daemons can be started with 
 sudo start carbon-cache-default-<instancename>

TODO:

- [x] Make carbon-relay do the same as carbon-cache #1
- [x] Finish the graphite-web classes so they can be customised #2
- [x] Remove unneeded start scripts #3
- [ ] Investigate upstart not using --debug to start carbon-cache without loosing pid
- [x] Upload debs somewhere
