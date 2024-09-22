Monitoring
==========

Create a Synthetic Monitoring
-----------------------------

.. code:: bash

   gcloud monitoring uptime create prod-api --synthetic-target https://example.com/api/v1/health

Create an Advanced Monitoring
-----------------------------

.. code:: bash

   gcloud monitoring uptime create prod-api \
      --resource-type=uptime-url \
      --resource-labels=host=example.com \
      --path /api/v1/health \
      --port 443 \
      --protocol https \
      --request-method get \
      --validate-ssl \
      --status-codes 200 \
      --period 1 \
      --regions usa-oregon asia-pacific usa-virginia \
      --timeout 10