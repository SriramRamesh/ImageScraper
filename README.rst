A cool command line app  which downloads all images in the given webpage. 

Download
--------

pip install
~~~~~~~~~~~

You can also download using pip:

.. code:: sh

    $ pip install ImageScraper

Usage
-----

.. code:: sh

    image-scraper [OPTIONS] URL

Options
-------

.. code:: sh

    -h, --help                      Print help
    -m, --max-images <number>       Maximum number images to be scraped
    -s, --save-dir  <path>          Name of the folder to save the images (default: ./images_<domain>)
    --max-filesize  <size>          Limit on size of image in bytes (default: 100000000)
    --dump-urls                     Print the URLs of the images

If you downloaded the tar:
~~~~~~~~~~~~~~~~~~~~~~~~~~

Extract the contents of the tar file. Note that ``ImageScraper`` depends
on ``lxml``. and ``requests``. If you run into problems in the
compilation of ``lxml`` through ``pip``, install the ``libxml2-dev`` and
``libxslt-dev`` packages on your system.

.. code:: sh

    $cd ImageScraper/
    $python setup.py install
    $image-scraper --max-images 10 [url to scrape]

If installed using pip:
~~~~~~~~~~~~~~~~~~~~~~~

Open python in terminal.

.. code:: sh

    $image-scraper --max-images 10 [url to scrape]

NOTE:
^^^^^

A new folder called "images_<domain>" will be created in the same place,
containing all the downloaded images.

