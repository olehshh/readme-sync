---
title: Get info of media inputs
excerpt: >
  Allows you to retrieve detailed information about the media inputs associated
  with a specific media item. You can use this endpoint to verify the media
  file’s input URL, track creation status, and container format. The mediaId
  (either uploadId or id) must be provided to fetch the information. 



  #### How it works




  Upon making a GET request with the mediaId, FastPix returns a response that
  includes: 


  * **Input-url:** The URL of the uploaded media file. 


  * **tracks:** Information about the tracks associated with the media,
  including both video and audio tracks, indicating whether they have been
  successfully created. 


  * **containerFormat:** The format of the uploaded media file container (e.g.,
  MP4, MKV). 

   

  This endpoint is particularly useful for ensuring that all necessary tracks
  (video and audio) have been correctly associated with the media during the
  upload or media creation process. 
api:
  file: api.json
  operationId: retrieveMediaInputInfo
hidden: false
---