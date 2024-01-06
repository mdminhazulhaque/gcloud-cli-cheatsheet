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