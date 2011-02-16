
Setting up Qt4 ruby and RUI on a Mac OS X
============================

Setup QT
--------

Installation of Qt4 and ruby bindings using Homebrew project.

	$ brew install dbus
	$ brew install qt --with-qtdbus
	$ for DIR in /usr/local/Cellar/qt/4.7.1/lib/*.framework; do ln -s /usr/local/Cellar/qt/4.7.1/lib/phonon.framework/Headers /usr/local/Cellar/qt/4.7.1/include/phonon; done

Make RVM gemset (optional)
-------------------------

I like to keep individual projects in separate RVM gemsets (no sharing of ruby gems).

	$ rvm use 1.9.2@projectX --create

Hello World!
-----------

	$ cd to/this/repo
	$ gem install bundler
	$ bundle install
	$ rake

Catharsis
---------

A new window with a push button should be staring back at you. Now get hacking!
