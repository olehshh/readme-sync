---
title: Get a media by ID
excerpt: >
  By calling this endpoint, you can retrieve detailed information about a
  specific media item, including its current status and a playbackId. This is
  particularly useful for retrieving specific media details when managing large
  content libraries. 




  #### How it works 




  1. Make a GET request to the **/media/{mediaId}** endpoint, replacing
  **{mediaId}** with the **uploadId** received during the upload process or the
  id obtained when creating media from a URL. 
   

  2. Receive a response that includes details about the media, including: 


  * **status:** Indicates whether the media is still “preparing” or has
  transitioned to "ready."  


  * **playbackId:** The playbackId is a unique identifier that allows you to
  stream the media once it is ready. You can construct the stream URL
  dynamically using the playbackId in the following format:
  https://stream.fastpix.io/${playbackId}.m3u8 

   

  **Please note:** Polling this API will let you know the status that whether
  the upload media has been moved to ready status, so that you can get started
  with streaming your media. 


  #### Use case scenario


  **Use case:** Suppose your platform provides users with an interface where
  they can manage their uploaded content. A user requests detailed information
  about a specific video to see if it has been fully processed and is available
  for playback. Using the media ID, you can fetch the information from FastPix
  and display it in the user’s dashboard. 
api:
  file: api.json
  operationId: get-media
hidden: false
---