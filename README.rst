The Knesset Meetings Corpus 2004-2005
=====================================
|DOI| |LICENCE| |PUBDOM|


A corpus of session protocols of the Knesset (Israeli parliament) between January 2004 and November 2005.


Contents
--------

The Knesset Meetings Corpus 2004-2005 is made up of two components:

* Raw texts - 282 files made up of 867,725 lines together. These can be downloaded in two formats:

  * As ``doc`` files, encoded using ``windows-1255`` encoding:

    * ``kneset16.zip`` - Contains 164 text files made up of 543,228 lines together. `[MILA host] <http://yeda.cs.technion.ac.il:8088/corpus/software/corpora/knesset/txt/docs/kneset16.zip>`_ `[Github Mirror] <https://github.com/NLPH/knesset-2004-2005/blob/master/kneset16.zip?raw=true>`_
  
    * ``kneset17.zip`` - Contains 118 text files made up of 324,497 lines together. `[MILA host] <http://yeda.cs.technion.ac.il:8088/corpus/software/corpora/knesset/txt/docs/kneset17.zip>`_ `[Github Mirror] <https://github.com/NLPH/knesset-2004-2005/blob/master/kneset17.zip?raw=true>`_
  
  * As ``txt`` files, encoded using ``utf8`` encoding:

    * ``kneset.tar.gz`` - An archive of all the raw text files, divided into two folders: `[Github mirror] <https://github.com/NLPH/knesset-2004-2005/blob/master/kneset.tar.gz>`_

      * ``16`` - Contains 164 text files made up of 543,228 lines together.
  
      * ``17`` - Contains 118 text files made up of 324,497 lines together.
    
    * ``knesset_txt_16.tar.gz``- Contains 164 text files made up of 543,228 lines together. `[MILA host] <http://yeda.cs.technion.ac.il:8088/corpus/software/corpora/knesset/txt/utf8/knesset_txt_16.tar.gz>`_ `[Github Mirror] <https://github.com/NLPH/knesset-2004-2005/blob/master/knesset_txt_16.tar.gz?raw=true>`_
    
    * ``knesset_txt_17.zip`` - Contains 118 text files made up of 324,497 lines together. `[MILA host] <http://yeda.cs.technion.ac.il:8088/corpus/software/corpora/knesset/txt/utf8/knesset_txt_17.zip>`_ `[Github Mirror] <https://github.com/NLPH/knesset-2004-2005/blob/master/knesset_txt_17.zip?raw=true>`_
 
* Tokenized and morphologically tagged texts - Tagged versions exist only for the files in the ``16`` folder. The text are represented using `MILA's XML schema for corpora <http://www.mila.cs.technion.ac.il/eng/resources_standards.html>`_. These can be downloaded in two ways:

  * ``knesset_tagged_16.tar.gz`` - An archive of all tokenized and tagged files. `[MILA host] <http://yeda.cs.technion.ac.il:8088/corpus/software/corpora/knesset/tagged/knesset_tagged_16.tar.gz>`_ `[Archive.org mirror] <https://archive.org/details/knesset_transcripts_2004_2005>`_
  
  * By cloning this repository, as the unarchived version of these files can be found in this repository, under the ``knesset_tagged`` folder.


Use
---

``txt`` format
--------------

These can be processed like any simple text file.

``doc`` format
--------------

Reading the ``doc``-formatted raw text files requires using a software supporting the ``windows-1255`` encoding.

For example, you can process these files using Python with the following code:

.. code-block:: python

  fpath = "/data/knesset/16/00133504.txt"
  with open(fpath, 'rt', encoding='windows-1255') as f:
    line = f.readline()
    # or with "for line in f", etc...
    
Mirrors
-------

This repository is a mirror of this dataset `found on MILA's website <http://www.mila.cs.technion.ac.il/eng/resources_corpora_haknesset.html>`_.

Zenodo mirror: `https://zenodo.org/record/2707356 <https://zenodo.org/record/2707356>`_
    
    
License
-------

All Knesset meeting protocols are in the `public domain <https://en.wikipedia.org/wiki/Public_domain>`_ (`רשות הציבור <https://he.wikipedia.org/wiki/%D7%A8%D7%A9%D7%95%D7%AA_%D7%94%D7%A6%D7%99%D7%91%D7%95%D7%A8>`_) by law. These files are thus in the public doamin and do not require any license or public domain dedication to set their status.

.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.2707356.svg
   :target: https://doi.org/10.5281/zenodo.2707356

.. |LICENCE| image:: https://github.com/NLPH/knesset-2004-2005/blob/master/public_domain_shield.svg
   :target: https://en.wikipedia.org/wiki/Public_domain

.. |PUBDOM| image:: https://github.com/NLPH/knesset-2004-2005/blob/master/public_domain.png
   :target: https://en.wikipedia.org/wiki/Public_domain
