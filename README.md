# Vagrant CoreOS Docker

 * Website: https://github.com/sthulb/vagrant-coreos-docker
 * Source: https://github.com/sthulb/vagrant-coreos-docker

A playground for creating Docker containers


# Installation

It's rather simple, clone and install Vagrant; or at least it was simple.

Vagrant 1.5 will support an rsync shared folder plugin, which currently doesn't
exist in the latest 1.4 release, I have however backported it. You can copy the
the plugin from the
[Vagrant](https://github.com/mitchellh/vagrant/tree/master/plugins/synced_folders/rsync)
repo. You will have to alter the `plugin.rb`.


# Usage

to get started just run: `vagrant up`


## Contributing

If you want to add functionality to this project, pull requests are welcome.

 * Create a branch based off master and do all of your changes with in it.
 * If it you have to pause to add a 'and' anywhere in the title, it should be two pull requests.
 * Make commits of logical units and describe them properly
 * Check for unnecessary whitespace with git diff --check before committing.
 * If possible, submit tests to your patch / new feature so it can be tested easily.
 * Assure nothing is broken by running all the test
 * Please ensure that it complies with coding standards.

**Please raise any issues with this project as a GitHub issue.**


## Credits

 * [@sthulb](https://twitter.com/sthulb)
