---
title: Get list of all media
excerpt: >
  This endpoint returns a list of all media files created from a URL or uploaded
  as file objects within your organization. Each media entry contains metadata
  such as the media ID, creation date, status, and type. It allows you to
  retrieve a comprehensive overview of your media assets, making it easier to
  manage and review them. 



  #### How it works


  When called, the API provides a paginated response containing the media items
  in the organization's library. This is helpful for retrieving a large volume
  of media and managing content in bulk. 




  #### Use case scenario 


  * **Use case:** A content manager at a video-on-demand platform wants to see
  all uploaded media to assess the quality and status of videos. 

   

  * **Detailed example:** 

  You're managing a video platform and need to check all the uploaded media in
  your library to ensure no outdated or low-quality content is being served.
  Using this endpoint, you can retrieve a complete list of media, allowing you
  to filter, sort, or update items as needed. 
api:
  file: api.json
  operationId: list-media
hidden: false
---