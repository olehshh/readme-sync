---
title: Update a media by ID
excerpt: >
  This endpoint allows you to update specific parameters of an existing media
  file. You can modify the key-value pairs of the metadata that were provided in
  the payload during the creation of media from a URL or when uploading the
  media as a file object. 



  #### How it works


  1. Make a PATCH request to the /media/{mediaId} endpoint, replacing {mediaId}
  with the uploadId or the id of the media you want to update. 


  2. Include the updated parameters in the request body. 


  3. Receive a response containing the updated media data, confirming the
  changes made. 
   
  Once you have made the update request, you can also look for the webhook event
  **video.media.updated** to notify your system about update status. 

   
  **Use case:** Imagine a scenario where a user uploads a video and later
  realizes they need to change the title, add a new description or tags. You can
  use this endpoint to update the media metadata without having to re-upload the
  entire video.
api:
  file: api.json
  operationId: updated-media
hidden: false
---