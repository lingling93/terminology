External Namespaces
===================
This directory contains namespaces generated from Bio2BEL packages. For an 
example of how they're used, see the `BEL Template <https://github.com/pharmacome/curation/blob/master/template.bel>`_.

Updating One
------------
1. Install the required Bio2BEL package with `pip`. This example uses 
   `Bio2BEL GO <https://github.com/bio2bel/go>`_:

.. code-block:: bash

   $ pip install bio2bel_go
   
2. Run the Bio2BEL GO command line. All repositories that can produce a 
   BEL identifiers namespace file have the subcommand `belns write`. 
   The `-f` flag can be used to specify the output path.

.. code-block:: bash

   $ bio2bel_go belns write -f go.belns
   
   
3. Use the `-n` flag to make a BEL names namespace file:

.. code-block:: bash

   $ bio2bel_go belns write -n -f go-names.belns

Updating All
------------
1. (Optional) Install additional Bio2BEL packages. This can be quickly
   done using the included ``requirements.txt`` file:

.. code-block:: bash

   $ pip install -r requirements.txt

2. Run the Bio2BEL batch BEL namespace writing command. The ``-d`` flag
   can be used to specify a directory that isn't the current working
   directory. This script takes care of both making identifiers and names
   files as well as naming them appropriately:

.. code-block:: bash

   $ bio2bel belns write
