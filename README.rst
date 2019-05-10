The Knesset Meetings Corpus 2004-2005
=====================================
|LICENCE|

A corpus of session protocols of the Knesset (Israeli parliament) between January 2004 and November 2005.


Contents
--------

The Knesset Meetings Corpus 2004-2005 is made up of two components:

* Raw texts - 282 files (encoded using the ``windows-1255`` encoding) made up of 867,725 lines together. These can be downloaded in two ways:

  * ``kneset.tar.gz`` - An archive of the raw text files, divided into two folders:

    * ``16`` - Contains 164 text files made up of 543,228 lines together.
  
    * ``17`` - Contains 118 text files made up of 324,497 lines together.
 
 * Each folder is also zipped separately into the ``kneset16.zip`` and the ``kneset17.zip`` files.
 
* Tokenized and morphologically tagged texts - Tagged versions exist only for the files in the ``16`` folder. The text are represented using `MILA's XML schema for corpora <http://www.mila.cs.technion.ac.il/eng/resources_standards.html>`_. These can be downloaded in two ways:

  * ``knesset_tagged_16.tar.gz`` - An archive of all tokenized and tagged files.
  
  * By cloning this repository, as the unarchived version of these files can be found in this repository, under the ``knesset_tagged`` folder.


Use
---

Reading the raw text files requires using a software supporting the ``windows-1255`` encoding.

For example, you can process these files using Python with the following code:

.. code-block:: python

  fpath = "/data/knesset/16/00133504.txt"
  with open(fpath, 'rt', encoding='windows-1255') as f:
    line = f.readline()
    # or with "for line in f", etc...
    
Mirrors
-------

This repository is a mirror of this dataset `found on MILA's website <http://www.mila.cs.technion.ac.il/eng/resources_corpora_haknesset.html>`_.
    
    
License
-------

All Knesset meeting protocols are in the `public domain <https://en.wikipedia.org/wiki/Public_domain>`_ (`רשות הציבור <https://he.wikipedia.org/wiki/%D7%A8%D7%A9%D7%95%D7%AA_%D7%94%D7%A6%D7%99%D7%91%D7%95%D7%A8>`_) by law. These files are thus in the public doamin and do not require any license or public domain dedication to set their status.
  
.. |LICENCE| image:: https://github.com/NLPH/knesset-2004-2005/blob/master/public_domain.png
  :height: 100px
  :scale: 20 %
  :target: https://en.wikipedia.org/wiki/Public_domain
