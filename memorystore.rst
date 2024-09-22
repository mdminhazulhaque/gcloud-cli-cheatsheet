MemoryStore
===========

List Redis
----------

.. code:: bash

   gcloud redis instances list --region us-west1

Create Redis
------------

.. code:: bash

   gcloud redis instances create dev-redis \
      --region us-west1 \
      --size 5 \
      --tier basic \
      --transit-encryption-mode disabled \
      --redis-version redis_6_x \
      --network dev-vpc \
      --connect-mode direct-peering

Get Redis Auth
--------------

.. code:: bash

   gcloud redis instances get-auth-string dev-redis --region us-east1