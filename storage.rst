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

   gcloud storage ls gs://dev-assets

Delete Object
-------------

.. code:: bash

   gcloud storage rm gs://dev-assets/dist/js/app.min.js

Copy From Local
---------------

.. code:: bash

   gcloud storage cp ./app.min.js gs://dev-assets/dist/js/app.min.js

Copy From Bucket
---------------

.. code:: bash

   gcloud storage cp gs://dev-assets/dist/js/app.min.js ./app.min.js

Create Public Bucket
--------------------

.. code:: bash

   gcloud storage buckets create gs://dev-assets --no-public-access-prevention

Create Public Object
--------------------

.. code:: bash

   gcloud storage objects update gs://dev-assets/dist/js/app.min.js --add-acl-grant=entity=allUsers,role=READER

Update Bucket CORS Policy
-------------------------

.. code:: bash

   gcloud storage buckets update gs://dev-assets --cors-file cors.json

.. code:: json

   [
      {
         "origin": ["https://example.com"],
         "method": ["GET"],
         "responseHeader": ["Content-Type"],
         "maxAgeSeconds": 3600
      }
   ]
