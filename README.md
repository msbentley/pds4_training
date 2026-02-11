# PDS4 training

This repo has a number of files and presentations used for the BepiColombo PDS4 training in Tokyo 11-12th February 2026.

## Contents

The contents of this repo are as follows:

- demos
  - a couple of python Jupyter notebooks using PSA/PDS APIs
- documentation
  - a PDF copy of the Bepi Annex to the PSA PDS4 archiving guide
  - a template for the archive Data User Guide
- example_products
  - some examples used in the workshop (PDS4 products)
- exercises
  - 1_validation
    - a set of exercises using the validate tool to identify and fix buggy products
  - 2_creating_products
    - a set of products (without labels) + a template to complete the File_Area
  - 3_creating_dictionary
    - a template IngestLDD file to use as the basis for adding new classes and attributes
  - 4_final
    - the final exercise adds new classes/attributes (from 3) to the output of exercise 2
- misc
  - a local_context_products.json file including Mio host and instruments, to run with validate
  - an example XML catalogue
- presentations
  - all presentations from the workshop

## Tools

In order to follow along with examples and demos, and to participate in the hands-on parts of the workshop, it is advisable for attendees to install some basic tools ahead of time. In particular we recommend that you set up:

- An XML-aware text editor or IDE
  - for example [VSCode](https://code.visualstudio.com/) or its open-source equivalent [VSCodium](https://vscodium.com/)
  - the most full-featured editor, which does Schemtron as well as schema validation, is [oXygen XML editor](https://www.oxygenxml.com/)
    - this is a commercial product, but a trial license key can be requested
- [validate](https://nasa-pds.github.io/validate/)
  - the PDS-provided validation tool used to check data and meta-data conformity
  - this requires java >= 17
- [LDDTool](https://nasa-pds.github.io/pds4-information-model/model-lddtool/index.html)
  - the PDS-provided tool to build local data dictionaries, needed for some hands-on activities
  - this requires java >= 17
- [PDS4 Viewer](https://sbnwiki.asteroiddata.org/PDS4_Viewer.html)
  - a tool to open/display any valid PDS4 data product
  - users who are familiar with python and tools such as conda may prefer to install [PDS4 Tools](https://sbnwiki.asteroiddata.org/Python_PDS4_Tools.html), the python library on which PDS4 viewer is based
    - PDS4 Tools is available in the conda-forge community repository

During the workshop we will also use GitHub to distribute templates, examples and other material. git experience is not necessary for this, but basic actions (such as cloning a repo) may make your life easier!

A [dockerfile](https://github.com/seignovert/pds4-workshop/) has also been created by one of the workshop participants to o install java, validate and lddtool in a single image.