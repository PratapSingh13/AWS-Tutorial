Go to the Services-->IAM-->Role and ***Create Role*** for **Lambda** in common used cases
 
![alt text](images/1.png "Title Text")

![alt text](images/2.png "Title Text")

Then again go into services-->DynamoDB and search for ***DynamoDB Full Access***

![alt text](images/3.png "Title Text")

Provide Role name whatever you want

![alt text](images/4.png "Title Text")

Here our Role is ready of named ***lambda-for-dynamodb***

![alt text](images/5.png "Title Text")

Go again into Services-->Lambda

![alt text](images/6.png "Title Text")

Create a Function

![alt text](images/7.png "Title Text")

Provide resspective details and select ***Use existing role*** because we have created our role earlier

![alt text](images/8.png "Title Text")

Here our Lambda Function created

![alt text](images/9.png "Title Text")

Go towards down into the page and put your code their here I'm using ***Edit code inline***

![alt text](images/10.png "Title Text")

This is our code 

![alt text](images/11.png "Title Text")

Now we need to create an AWS S3 Bucket to add trigger
Go to the Services-->S3

![alt text](images/12.png "Title Text")

Here I create my S3 Bucket of named ***pratap.s3.bucket***

![alt text](images/13.png "Title Text")

Now if we go on to **Add trigger** in our Lambda we get the S3 option 

![alt text](images/14.png "Title Text")

Here in trigger section I choosed ***All object create event*** it basically fire trigger in every situation
***Note-:*** Trigger must be checked as Enabled

Now time to create **DynamoDB** in services-->DynamoDB

![alt text](images/15.png "Title Text")

Create Table as named you choose in your Python Code and also with Primary key as same as in Python Code
In my case I take myTable as Table name and uniqueID as Primary Key

![alt text](images/16.png "Title Text")

![alt text](images/17.png "Title Text")

Here our Table is created 

![alt text](images/18.png "Title Text")

Now we need to upload any type of file in our S3 bucket to test that our lambda is working or not
So here i uploaded my two of files 

![alt text](images/19.png "Title Text")


![alt text](images/20.png "Title Text")

Now go to the DynamoDB and select Table and choose your table name-->Item
**And The BAR IS SET!**
You can see every details of your data like type of file, put/post/get, size etc.

![alt text](images/21.png "Title Text")


### Contributors
[![Yogendra Pratap Singh][yogendra_avatar]][yogendra_homepage]<br/>[Yogendra Pratap Singh][yogendra_homepage] 

  [yogendra_homepage]: https://github.com/PratapSingh13
  [yogendra_avatar]: https://img.cloudposse.com/75x75/https://github.com/PratapSingh13.png
