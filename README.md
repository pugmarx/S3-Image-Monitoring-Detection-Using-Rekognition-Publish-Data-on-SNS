# S3-Image-Monitoring-Detection-Using-Rekognition-Publish-Data-on-SNS
AWS Serverless application for S3 Images Monitoring. Detect Image using AWS rekognition API and publish data on SNS


# Inspiration
To detect images posted on internet, S3 buckets, website based on it content, text which we may want to use or we want to detect if any image is unsafe or inappropriate. I need an application which can easily find properties to analyse and detect images which I want to find.

# What it does
This application has two use, first is it can be used to identify images which are unsafe , inappropriate , has adult content and then we can block/remove those images. On other hand if we have lot if images then based and we are looking for images which has some certain contents e.g. Train, river, house then we can detect labels of images and identify the image of our use.

# How I built it
I have built this application using AWS SAM , When we have images on any application , website etc, these images can be directed to be saved on "S3 Bucket' . On image upload S3 bucket triggers Lambda function to execute the code. This lambda function utilises rekognition API to analyse the uploaded image and finds the Image Labels, Text contained by the image and most importantly Moderation Labels. Then this all data is formatted and published on SNS Topic , If any user has subscribed this topic , will get notification and the user can review the image contents and properties and where the image is location on S3 Bucket.

# Challenges I ran into
It was tough to learn AWS SAM completely from scratch .It was really difficult to debug the application when so many types of resources are involves

# Accomplishments that I'm proud of
I have successfully deployed a complete application which utilises so many resources from AWS and I can help people finding unwanted images. Which may further help preventing Human Trafficking

# What I learned
I have learned SNS, S3, SAM Templates , Lambda to publish this application

# What's next for Image Detection by Rekognition API and Publish on SNS
Face comparison, Collage preparation , Image Conversion and Live Video Detection from CCTV Cameras

# Built With
amazon-web-services, sam, s3 ,lambda ,rekognition , sns, python
