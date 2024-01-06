gcloud CLI Cheatsheet
=====================

Supercharge your daily acitivities related to GCP using the combination of `gcloud`` CLI and `jq`.

Prerequisites
-------------

-  `gcloud-cli <https://cloud.google.com/sdk/docs/install-sdk/>`__
-  `jq <https://stedolan.github.io/jq/>`__

|:warning:| Disclaimer: All Resource Name, Account, Hostname etc are
generated using `Faker <https://faker.readthedocs.io/en/master>`__. They
should not match any real user data.

|:arrow_right:| If you have multiple GCP Projects, you can use export variables
to point gcloud to specific Project, Region and Zone.

.. code:: bash

   export CLOUDSDK_CORE_PROJECT=my-dev-project
   export CLOUDSDK_COMPUTE_REGION=us-west1
   export CLOUDSDK_COMPUTE_ZONE=us-west1-c

.. toctree::
   :caption: GCloud Commands
   :maxdepth: 100
   :hidden:

   artifacts
   compute
   container
   storage
