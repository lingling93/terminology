External Namespaces
===================
This directory contains namespaces generated from Bio2BEL packages.

1. (Optional) Install additional Bio2BEL packages. This can be quickly
   done using the included ``requirements.txt`` file:

.. code-block:: bash

   $ pip install -r requirements.txt

2. Run the Bio2BEL batch BEL namespace writing command. The ``-d`` flag
   can be used to specify a directory that isn't the current working
   directory:

.. code-block:: bash

   $ bio2bel belns write