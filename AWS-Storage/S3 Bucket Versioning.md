## AWS S3 Bucket Versioning ##

- Bucket Versioning is a S3 Bucket sub-resource used to protect against accidental object/data deleted or overwrite.
(If we enable versioning then if we deleted our data by mistake then it does not deleted but it becomes **delete marker** and in future we can restore that data again Just like case of recycle bin)

- Versioning is also used for data retention and archive.

- Once we enable versioning on a bucket it can not be disable however it can be suspended.

- When enabled, Bucket versioning will protect existing and new objects, and maintains their versions as they are updated.

- Versioning enabled on bucket not on object.

- Updating objects refers to PUT, POST, COPY, DELETE actions on object.

- When versioning is enabled and you try to delete an object, a delete marker is placed on the object.
  - You can still view the object and the delete marker.

- If you re-consider deleting the objects, you can delete the **Delete Marker** and the object will be available again.

- You will be charge for all S3 storage cost for all object versions stored.

- You can use versioning with S3 lifecycle policies to delete older versions or you can move them to a cheaper S3 storage (or Glacier).

- Bucket versioning state:
  - Enabled
  - Suspended
  - Un-Versioned (It automatically disappear when we enable versioning because we can not disable it)

- Versioning applies to all objects in a bucket and not partially applied.

- Object existing before enabling versioning will have a version ID NULL.

- If you have a bucket that is already versioned then you suspend versioning existing object and their version remain as it is.

- However they will not be updated version further with future updates while the bucket versioning is suspended.

- New objects they will have version ID NULL id versioning is suspended.

- An oject deletion in a suspended versioning bucket will only delete the object with ID NULL.



### Contributors
[![Yogendra Pratap Singh][yogendra_avatar]][yogendra_homepage]<br/>[Yogendra Pratap Singh][yogendra_homepage] 

  [yogendra_homepage]: https://github.com/PratapSingh13
  [yogendra_avatar]: https://img.cloudposse.com/75x75/https://github.com/PratapSingh13.png



















