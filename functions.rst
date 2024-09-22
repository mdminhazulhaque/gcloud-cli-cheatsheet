Cloud Functions
===============

List Functions
--------------

.. code:: bash

   gcloud functions list --format "table(name)"

Deploy Function
---------------

.. code:: bash

   gcloud functions deploy prod-app \
      --memory 256MB \
      --runtime python39 \
      --trigger-http \
      --entry-point hello_world \
      --max-instances 100 \
      --source ./ \
      --gen2 \
      --region us-east1
