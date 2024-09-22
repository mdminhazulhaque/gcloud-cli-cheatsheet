Container
=========

List Clusters
-------------

.. code:: bash

   gcloud container clusters list --format "table(name)"

.. code:: ini

   NAME
   prod-clsuter
   stage-clsuter
   dev-clsuter

Update KUBECONFIG for a Clusters
--------------------------------

.. code:: bash

   gcloud container clusters get-credentials prod-clsuter

.. code:: ini

   Fetching cluster endpoint and auth data.
   kubeconfig entry generated for prod-clsuter.

List GKE Maintenance Operations
-------------------------------

.. code:: bash

   gcloud container operations list

Describe GKE Maintenance Operation
----------------------------------

.. code:: bash

   gcloud container operations describe operation-172000000000-EC9B4B2F-53B9-4AAA-AA0A-3BF16FDE03C2

