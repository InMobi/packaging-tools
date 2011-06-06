build-package
===========

Description
-----------

A wrapper around dpkg-deb to build Debian .deb packages

Requirements
------------

* Tested on Ubuntu 10.04 LTS
* dpkg-dev
* libyaml-syck-perl

Installation & Usage
--------------------

1.  $ mkdir ~/build-pachage/

2.  Create build-package/config.yaml with the following contents

	package: build-package
	version: 0.1.0
	arch: all
	maintainer: Shanker Balan <shanker.balan@inmobi.com>
	description: Hack to build a .deb using a YAML config
	predepends: dpkg-dev, libyaml-syck-perl
	section: ops

3.  mkdir -p ~/build-package/usr/bin/

4.  Drop the build-package perl script into ~/build-package/usr/bin folder

5.  Now bootstrap

	$ cd ~/build-package
	$ build-package

6.  dpkg -i build-package-x.y.x-xxxxxxxx.deb

Issues
------

Possibly many.

Author
------

Shanker Balan <shanker.balan@inmobi.com>

License
-------

    Author:: Shanker Balan (<shanker.balan@inmobi.com>)
    Copyright:: Copyright (c) 2011 InMobi
    License:: The BSD License


	Copyright (c) 2011, Shanker Balan
	All rights reserved.

	Redistribution and use in source and binary forms, with or without
	modification, are permitted provided that the following conditions are met:
	Redistributions of source code must retain the above copyright notice, this
	list of conditions and the following disclaimer.  Redistributions in binary
	form must reproduce the above copyright notice, this list of conditions and the
	following disclaimer in the documentation and/or other materials provided with
	the distribution.

	THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
	ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
	WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
	DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
	FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
	DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
	SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
	CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
	OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
	OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
