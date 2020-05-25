## AWS Storage ##
### Storage ###
Where we are storing our data is called Storage
### Types of Storage in AWS ###
- *Amazon Simple Storage Service (Amazon S3)*
- *Amazon Elastic File System (Amazon EFS)*
- *Amazon Elastic Block Storage (Amazon EBS)*
- *Amazon Glacier*
- *Amazon Snowball*
- *Amazon CloudFront*

### Block Storage vs Object Storage ###
### Block Storage ###
- Block Storage is suitable for transactional databases, random read & write loads and structure database storage.
(Block Storage is good for structural databse where we need to do parallel processing)
- Block Storage divides data to be stored in evenly sized blocks for instance a file can be split into evenly sized blocks before it is stored
- Data Block stored in block storage would not contain meta data (Meta data is not for block it is for complete data meta data).
- Block storage only keeps the address(index) where the data blocks are stored, it does not care what is in that Block, just know how to retrieve it when required.

### Object Storage ###
- Object Storage stores the files as a whole and does not divide them.
- In object storage an object is
  - The file/data it self
  - Meta Data
  - Object Global unique ID
- The object Global Uniquee ID, is unique identifier for the object (can be the object's name itself and it must be unique such that it can be retrieved disregarding where its physical storage location is.
- Object storage can not be mounted as drive.
  
