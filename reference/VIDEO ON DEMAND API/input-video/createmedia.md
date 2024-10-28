---
title: Create media from URL
excerpt: >
  This endpoint allows developers or users to create a new video or audio media
  in FastPix using a publicly accessible URL. FastPix will fetch the media from
  the provided URL, process it, and store it on the platform for use. 




  #### Public URL requirement:


    The provided URL must be publicly accessible and should point to a video stored in one of the following supported formats: .m4v, .ogv, .mpeg, .mov, .3gp, .f4v, .rm, .ts, .wtv, .avi, .mp4, .wmv, .webm, .mts, .vob, .mxf, asf, m2ts 

   

  #### Supported storage types:


  The URL can originate from various cloud storage services or content delivery
  networks (CDNs) such as: 



  * **Amazon S3:** URLs from Amazon's Simple Storage Service. 


  * **Google Cloud Storage:** URLs from Google Cloud's storage solution. 


  * **Azure Blob Storage:** URLs from Microsoft's Azure storage. 


  * **Public CDNs:** URLs from public content delivery networks that host video
  files. 


  Upon successful creation, the API returns an id that should be retained for
  future operations related to this media. 
   
  #### How it works
   

  1. Send a POST request to the /media endpoint with the media URL (typically a
  video or audio file) and optional media settings. 


  2. FastPix uploads the video from the provided URL to its storage. 


  3. Receive a response containing the unique id for the newly created media
  item. 


  4. Use the id in subsequent API calls, such as checking the status of the
  media with the **Get Media by ID** endpoint to determine when the media is
  ready for playback. 


  FastPix uses webhooks to tell your application about things that happen in the
  background, outside of the API regular request flow. For instance, once the
  media file is created (but not yet processed or encoded), we’ll shoot a POST
  message to the address you give us with the webhook event
  video.media.created. 



  Once processing is done you can look for the events video.media.ready and
  video.media.failed to see the status of your new media file.


  #### Use case scenario
   

  * **Use case:** A developer wants to integrate a user-generated content
  platform where users can upload links to their videos hosted on third-party
  platforms like AWS or Google Cloud Storage. This endpoint is used to create
  media directly from those URLs. 



  * **Detailed example:** 

  Say you’re building an online learning platform where instructors upload video
  URLs hosted on their private cloud servers. By providing the video URL to this
  endpoint, the platform processes and adds it to your media library, ready for
  playback. 
api:
  file: api.json
  operationId: create-media
hidden: false
---
sss