---
title: Alert Uploads
excerpt: >-
  This endpoint allows you to upload Alert requests with more than 2MB of data.
  It involves a 4-step client flow: 1. Request an upload URL by calling the POST
  /alert_uploads endpoint. The request body should be an empty JSON object. 2.
  Upload your encrypted alerts data to the provided URL. 3. Notify the server
  that your upload is complete by calling the PUT
  /alerts_uploads/{token}/complete endpoint. 4. Poll for the outcome of the
  upload by calling the GET /alert_uploads/{token} endpoint. To see how to
  encrypt your Alerts request body and upload to S3, see this [help center
  article]
  (https://help.hummingbird.co/hummingbird-api/how-do-i-upload-larger-alerts-data-via-api)
api:
  file: oas.json
  operationId: alert_uploads_post
hidden: false
---