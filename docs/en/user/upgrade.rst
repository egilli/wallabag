Upgrade wallabag
================

Upgrade on a dedicated web server
---------------------------------

The last release is published on https://www.wallabag.org/pages/download-wallabag.html. In order to upgrade your wallabag installation and get the last version, run the following commands in you wallabag folder (replace ``2.1.0`` by the last release number):

::

    git fetch origin
    git fetch --tags
    git checkout 2.1.0
    ./install.sh

Upgrade on a shared hosting 
---------------------------

Backup your ``app/config/parameters.yml`` file.

Download the last release of wallabag: 

.. code-block:: bash

    wget http://wllbg.org/latest-v2-package && tar xvf latest-v2-package

Extract the archive in your wallabag folder and replace ``app/config/parameters.yml`` with yours.

If you use SQLite, you must also copy your ``data/`` folder inside the new installation.

Empty ``var/cache`` folder.
