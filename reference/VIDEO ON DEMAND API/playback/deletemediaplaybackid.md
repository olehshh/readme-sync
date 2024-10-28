---
title: Delete a playback ID
excerpt: >
  This endpoint allows you to remove a specific playback ID associated with a
  media asset. Deleting a playbackId will revoke access to the media content
  linked to that ID. 



  #### How it works


  1. Make a DELETE request to the /on-demand/{mediaId}/playback-ids endpoint,
  replacing {mediaId} with the uploadId or id of the media asset from which you
  want to delete the playback ID. 


  2. Specify the playback ID you wish to delete in the request body. 


  **Use case:** Your platform offers limited-time access to premium content.
  When the subscription expires, you can revoke access to the content by
  deleting the associated playback ID, preventing users from streaming the video
  further. 
api:
  file: api.json
  operationId: delete-media-playback-id
hidden: false
---