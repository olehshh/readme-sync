---
title: Upload media from device
excerpt: >
  This endpoint allows you to upload a video file directly from your local
  device to FastPix for processing and storage. By calling this API with your
  preferred media settings, you will receive an uploadId and a pre-signed url in
  the response. 




  #### How it works


  1. Send a POST request to the /uploads endpoint with optional media
  settings.  


  2. Receive a response containing the **uploadId** and a pre-signed **URL** for
  uploading your video file.  


  3. Upload your video file to the provided **URL** by making **PUT** request.
  The API accepts the media file from the device and uploads it to the FastPix
  platform. 


  4. Once uploaded, the media undergoes processing and is assigned a unique ID
  for tracking. Retain this **uploadId** for any future operations related to
  this upload. 





  After uploading, you can use the **Get Media by ID** endpoint to check the
  status of the uploaded media asset and see if it has transitioned to a "ready"
  status for playback. 


  To notify your application about the status of this API request check for the
  webhooks for Upload related events.  

   
  #### Use case scenario 


  **Use case:** A social media platform lets users upload video content directly
  from their phones or computers. This endpoint handles the upload process. For
  instance, if you're building a video-sharing app where users can upload short
  clips from their mobile devices. Using this endpoint, users can select a video
  from their device, upload it to the platform, and have it processed for
  playback on the app. 
api:
  file: api.json
  operationId: direct-upload-video-media
hidden: false
---