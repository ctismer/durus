Durus Installation
==================

Requirements:
-------------

Durus requires Python version 2.6 or above.
Python distributions are available at http://www.python.org.
If you need to run Durus on Windows NT/2000, you will need
python with the win32 extensions, available at
http://sf.net/projects/pywin32/.
Durus includes an optional C-extension that makes it run much
faster.  You will need a C compiler to build the extension.


Installation:
-------------

Go to http://www.mems-exchange.org/software/durus and download the
latest version.
Untar the tarball with a command like this::

    tar zvxf Durus-3.9.3.tar.gz

Move into the Durus source directory::

    cd Durus-3.9.3

Here is the standard installation command, with the additional option
that creates a "durus.installed" file containing the list of installed
files::

    python setup.py install --record installed.txt

Watch the install messages for "permission denied" warnings: if you
see any, it probably means that you don"t have write permission on the
"site-packages" directory in the installed python lib directory, or
else on the installed python bin directory.  You can either change the
permissions on those directories or else you can try a customized
installation.

Review the installed.txt file to see where the install script made
changes.  You should make sure that the script files installed to the python
bin directory are on your command shell's path.


Customized Installation:
------------------------

To see all of the install options, run this command::

    python setup.py install --help
    
