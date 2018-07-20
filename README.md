Requirements:
-------------------------
Generic:
* Digibyte >=6.14.2
* Python >=2.6
* Twisted >=10.0.0
* python-argparse (for Python =2.6)

Linux:
* sudo apt-get install python-zope.interface python-twisted python-twisted-web
* sudo apt-get install python-argparse # if on Python 2.6

Windows:
* Install Python 2.7: http://www.python.org/getit/
* Install Twisted: http://twistedmatrix.com/trac/wiki/Downloads
* Install Zope.Interface: http://pypi.python.org/pypi/zope.interface/3.8.0
* Install python win32 api: http://sourceforge.net/projects/pywin32/files/pywin32/Build%20218/
* Install python win32 api wmi wrapper: https://pypi.python.org/pypi/WMI/#downloads
* Unzip the files into C:\Python27\Lib\site-packages

Official wiki:
-------------------------
https://en.bitcoin.it/wiki/P2Pool

Alternate web frontend:
-------------------------
* https://github.com/hardcpp/P2PoolExtendedFrontEnd

Notes for Digibyte:
=========================
In order to run Digibyte nodes you must first install the digibyte_subsidy & python_skein_hash modules:
-------------------------
    git submodule init
    git submodule update
    cd digibyte_subsidy
    sudo python setup.py install
    cd ..
    cd python_skein_hash
    sudo python setup.py install

Running P2Pool:
-------------------------
To use P2Pool, you must be running your own local myriadcoind. For standard configurations, using P2Pool should be as simple as:

    python run_p2pool.py --net digibyte

To make your node accessible from the internet, open the following ports on your router (both the worker port and peer-2-peer port please!): Worker Port = 5029; Peer-2-Peer Port = 5028

Run for additional options:

python run_p2pool.py --help

Donations towards further development:
-------------------------
BTC: 1HNeqi3pJRNvXybNX4FKzZgYJsdTSqJTbk 17Vq6qwfE1epzsgEfSw81pQX3gXo9ZN4ET
DGB: DTvN7hB8dXEVLNjvEkCaEm34AXb8LpxmKM
