---
title: Complete Upload
excerpt: >-
  Notify the server that the alert upload has been completed on your side. Send
  an empty JSON object {}. Use the token obtained from the response to the
  initial GET request. The server will will synchronously verify that the
  uploaded file exists in S3 and enqueue for further processing. No other
  verification or processing will occur as a result of this call.
api:
  file: oas.json
  operationId: alert_uploads_complete_put
hidden: false
---