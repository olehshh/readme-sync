---
title: Delete a media by ID
excerpt: >
  This endpoint allows you to permanently delete a a specific video or audio
  media file along with all associated data. If you wish to remove a media file
  from FastPix storage, use this endpoint with the **mediaId** (either
  **uploadId** or **id**) received during the media's creation or upload. 



  #### How it works



  1. Make a DELETE request to the /media/{mediaId} endpoint, replacing {mediaId}
  with the uploadId or the id of the media you want to delete. 


  2. Confirm the deletion: Since this action is irreversible, ensure that you no
  longer need the media before proceeding. Once deleted, the media cannot be
  retrieved or played back. 


  3. Webhook event to look for: **video.media.deleted** 


  **Use case:** A user on a video-sharing platform decides to remove an old
  video from their profile, or suppose you're running a content moderation
  system, and one of the videos uploaded by a user violates your platform’s
  policies. Using this endpoint, the media is permanently deleted from your
  library, ensuring it’s no longer accessible or viewable by other users. 
api:
  file: api.json
  operationId: delete-media
hidden: false
---