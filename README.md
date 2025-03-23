# [Archived] Ansible Collection - tronde.wordpress

_Notice:_ This repository has been archived as future work is going to happen at [codeberg.org](https://codeberg.org) in [https://codeberg.org/Tronde/wordpress](https://codeberg.org/Tronde/wordpress).

This collection contains three roles for the following use cases:

  * Install Wordpress to some host
  * Backup Wordpress files and database
  * Restore Wordpress files and database

The documentation for the roles in included in the README.md of the respective
role.

I'll use the prefix 'wp' as short form for Wordpress in role and variable
names.

Please take a look at the commit messages and release notes (if there are any releases) to get an idea about the current status.

## Supported platforms

Currently this collection is tested against:

  * Debian 12 (Bookworm)

In the futrure I would like to add support for the following distributions:

  * Red Hat Enterprise Linux (RHEL) 9
  * Ubuntu LTS
  * Fedora

## Contributing

Wordpress is a blogging platform and CMS widely in use. I believe that this
Ansible collection provides some value to the community. As I'm only a single
individuum with limited time, I would be happy if you would like to contribute
to this collection.

The role is developed with the [Ansible Good Practices](https://redhat-cop.github.io/automation-good-practices/) in mind. Please,
ensure that your Pull Requests follows these guidelines to be accepted.

Any feedback is welcome. Please use the issue tracker or drop me an email.
