Compute
=======

List Instances
--------------

.. code:: bash

   gcloud compute instances list --format "table(NAME,EXTERNAL_IP)"
   
.. code:: ini

   NAME                     EXTERNAL_IP
   dev-app-23592f07-qypx    35.200.50.100
   prod-app-5813e6e2-r5xg   35.200.50.101
   stage-app-d82edb97-ioot  35.200.50.102
   
SSH into an Instance
--------------------

.. code:: bash

   gcloud compute ssh dev-app-23592f07-qypx
