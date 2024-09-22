Artifacts
=========

List Repositories
-----------------

.. code:: bash

   gcloud artifacts repositories list --format "table(name)"

.. code:: ini

   NAME
   prod-frontend
   prod-backend
   prod-middleware

Create Repository
-----------------

.. code:: bash

   gcloud artifacts repositories create prod-frontend --repository-format docker --location us-west1

List Images
-----------

.. code:: bash

   gcloud artifacts docker images list us-west1-docker-pkg.dev/my-proj-name/prod-frontend

Configure Docker and Push Image
-------------------------------

.. code:: bash

   gcloud auth configure-docker us-west1-docker-pkg.dev
   docker tag app:latest us-west1-docker-pkg.dev/my-proj-name/prod-frontend:latest
   docker push us-west1-docker-pkg.dev/my-proj-name/prod-frontend:latest