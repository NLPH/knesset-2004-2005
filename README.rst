Knesset Meetings 2004-2005
==========================

A corpus of transcriptions of Knesset (Israeli parliament) meetings between January 2004 and November 2005.


Contents
========

* ``kneset.tar.gz`` - An archive of raw text files (encoded using the ``windows-1255`` encoding), divided into two folders:

  * ``16`` - Contains 164 text files made up of 543,228 lines together.
  
  * ``17`` - Contains 118 text files made up of 324,497 lines together.

* ``knesset_tagged_16.tar.gz`` - An archive of tokenized and morphologically tagged XML versions of all files in the ``16`` folder. The text are represented using `MILA's XML schema for corpora <http://www.mila.cs.technion.ac.il/eng/resources_standards.html>`_.

Use
===

Reading the raw text files requires using a software supporting the ``windows-1255`` encoding.

For example, you can process these files using Python with the following code:

.. code-block:: python

  fpath = "/data/knesset/16/00133504.txt"
  with open(fpath, 'rt', encoding='windows-1255') as f:
    line = f.readline()
    # or with "for line in f", etc...
    
    
License
=======

All Knesset meeting protocols are in the `public domain <https://en.wikipedia.org/wiki/Public_domain>`_ (`רשות הציבור <https://he.wikipedia.org/wiki/%D7%A8%D7%A9%D7%95%D7%AA_%D7%94%D7%A6%D7%99%D7%91%D7%95%D7%A8>`_) by law. Thus this files are in the public doamin and do not require any license or public domain dedication to set their status.
  
