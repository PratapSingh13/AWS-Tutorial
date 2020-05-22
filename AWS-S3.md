### AWS S3 ###
- S3 stands for **Simple Storage Service**
- S3 is a storage for the internet it has a simple web services interface for simple storing & retrieving of any amount of data anytime from anywhere on the internet.
- S3 is object based storage.
- You can not install OS on S3.
- S3 has a distributed data store architecture where objects are redundantly stored in multiple locations.
- Data is stored in Bucket.
- A Bucket is a flat container of object (We can not make bucket inside bucket).
- Max capacity of a Bucket is 5TB.
- You can create folders in your bucket (available through console).
- You can not create nested Bucket.
- Bucket ownership is non-transferable.
- S3 Bucket is region specific.
- You can have upto 100 Buckets per account (may be expanded).

### S3 Bucket naming rules ###
- S3 Bucket name are globally unique across all AWS.
- Bucket name can not be change after creation.
- If a bucket is deleted, the name becomes available again to you or for another account.
- Bucket name must be atleast 3 and not more than 63 characters.
- Bucket names are part of the URL used to access to the Bucket.
- Bucket name must be the series of one or more labels.
- Bucket name can contain lowercase, number, and hyphen but can not use Uppercase letter.
- Bucket name should not be an IP address.
- Each label must start and end with a lowercase letter or a number.
- By default buckets and its object are private only owner can access the bucket.

### S3 Bucket sub-resurces ###
#### Sub-Resources for S3 bucket includes: ####
**Lifecycle-** To decide an object lifecycle management.
**Website-** To hold configuration related to static website hosted in S3 bucket.
**Versioning-** Keep object versions as it changes (We can not disable Versioning only we can either enable or suspend it).
**Access Control List-** Bucket accessibility.
