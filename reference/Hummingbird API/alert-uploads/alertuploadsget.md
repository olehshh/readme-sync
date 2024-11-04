---
title: Fetch status
excerpt: >-
  This endpoint can be polled for the results of the upload. It returns the
  overall status of the alert (and an error message if one occurred), as well as
  an array of AlertFetchResponse objects (the same response typically provided
  by the GET /alerts/{token} endpoint on a per-alert basis). The array of alerts
  will remain EMPTY until ALL alerts in the upload have been processed, and the
  status is either PROCESSED or ERROR.
api:
  file: oas.json
  operationId: alert_uploads_get
hidden: false
---