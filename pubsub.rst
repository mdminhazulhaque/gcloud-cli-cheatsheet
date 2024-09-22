Pub/Sub
=======

List Topics
-----------

.. code:: bash

   gcloud pubsub topics list --format "table(name)"

List Subscriptions
------------------

.. code:: bash

   gcloud pubsub subscriptions list --format "table(name, topic)"

Create Topic
------------

.. code:: bash

   gcloud pubsub topics create prod-app-pub

Create Subscription
-------------------

.. code:: bash

   gcloud pubsub subscriptions create prod-app-sub --topic prod-app-pub
