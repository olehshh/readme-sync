---
title: Create a playback ID
excerpt: >
  You can create a new playback ID for a specific media asset. If you have
  already retrieved an existing playbackId using the "Get Media by ID" endpoint
  for a media asset, you can use this endpoint to generate a new playback ID
  with a specified access policy. 




  If you want to create a private playback ID for a media asset that already has
  a public playback ID, this endpoint also allows you to do so by specifying the
  desired access policy. 


  #### How it works 
   
  1. **Make a POST request** to the /on-demand/{mediaId}/playback-ids endpoint,
  replacing {mediaId} with the uploadId or id of the media asset. 


  2. Include the **access policy** in the request body to indicate whether the
  new playback ID should be private or public. 


  3. Receive a response containing the newly created playback ID with the
  requested access level. 



  **Use case:** A video streaming service generates playback IDs for each media
  file when users request to view specific content. The playback ID is then used
  by the video player to stream the video. 
api:
  file: api.json
  operationId: create-media-playback-id
hidden: false
---