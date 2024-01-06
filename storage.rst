Storage
=======

List Buckets
------------

.. code:: bash

   gcloud storage buckets list --format "table(name)"

.. code:: ini

   NAME
   dev-assets
   stage-assets
   prod-assets
   terraform-state

List Objects
------------

.. code:: bash

   gcloud storage objects list gs://dev-assets