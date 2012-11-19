Description
===========

Sets the default system locale.

List the available locales:

	$ locale -a 

Ubuntu/Debian tools require different locale environment settings beyond "LANG".

Instead of using 'update-locale', this script gets paranoid and updates all possible locale defaults in /etc/default/locale. This solves errors like:

* unsupported locale setting
* Gtk-WARNING **: Locale not supported by C library

Requirements
============

Tested on Ubuntu >= 10.04, Debian Squeeze

Attributes
==========

* `node[:locale]` -- defaults to "en_US.utf8"

Usage
=====

Include the default recipe in your run list.