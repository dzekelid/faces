---
name: AWS Rekognition
x-slug: aws-rekognition
description: Amazon Rekognition is a service that makes it easy to add image analysis
  to your applications. With Rekognition, you can detect objects, scenes, and faces
  in images. You can also search and compare faces. Rekognition&rsquo;s API enables
  you to quickly add sophisticated deep learning-based visual search and image classification
  to your applications.Amazon Rekognition is based on the same proven, highly scalable,
  deep learning technology developed by Amazon&rsquo;s computer vision scientists
  to analyze billions of images daily for Prime Photos. Amazon Rekognition uses deep
  neural network models to detect and label thousands of objects and scenes in your
  images, and we are continually adding new labels and facial recognition features
  to the service.Rekognition&rsquo;s API lets you easily build powerful visual search
  and discovery into your applications. With Amazon Rekognition, you only pay for
  the images you analyze and the face metadata you store. There are no minimum fees
  and there are no upfront commitments.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
x-kinRank: "10"
x-alexaRank: ""
tags: Faces
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Rekognition API Compare Faces
  x-api-slug: aws-rekognition-api
  description: |-
    Compares a face in the source input image with
          each face detected in the target input image.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
  humanURL: https://aws.amazon.com/rekognition/
  baseURL: ://///?Action=CompareFaces
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/actioncomparefaces-get-openapi.md
- name: AWS Rekognition API Delete Faces
  x-api-slug: aws-rekognition-api
  description: Deletes faces from a collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
  humanURL: https://aws.amazon.com/rekognition/
  baseURL: ://///?Action=DeleteFaces
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/actiondeletefaces-get-openapi.md
- name: AWS Rekognition API Detect Faces
  x-api-slug: aws-rekognition-api
  description: Detects faces within an image (JPEG or PNG) that is provided as input.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
  humanURL: https://aws.amazon.com/rekognition/
  baseURL: ://///?Action=DetectFaces
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/actiondetectfaces-get-openapi.md
- name: AWS Rekognition API Index Faces
  x-api-slug: aws-rekognition-api
  description: Detects faces in the input image and adds them to the specified collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
  humanURL: https://aws.amazon.com/rekognition/
  baseURL: ://///?Action=IndexFaces
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/actionindexfaces-get-openapi.md
- name: AWS Rekognition API List Faces
  x-api-slug: aws-rekognition-api
  description: Returns metadata for faces in the specified collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
  humanURL: https://aws.amazon.com/rekognition/
  baseURL: ://///?Action=ListFaces
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/actionlistfaces-get-openapi.md
- name: AWS Rekognition API Search Faces
  x-api-slug: aws-rekognition-api
  description: For a given input face ID, searches for matching faces in the collection
    the face belongs to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
  humanURL: https://aws.amazon.com/rekognition/
  baseURL: ://///?Action=SearchFaces
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/actionsearchfaces-get-openapi.md
- name: AWS Rekognition API Search Faces By Image
  x-api-slug: aws-rekognition-api
  description: |-
    For a given input image, first detects the largest face in the image, and
          then searches the specified collection for matching faces.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
  humanURL: https://aws.amazon.com/rekognition/
  baseURL: ://///?Action=SearchFacesByImage
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/actionsearchfacesbyimage-get-openapi.md
- name: AWS Rekognition API
  x-api-slug: aws-rekognition-api
  description: Amazon Rekognition is a service that makes it easy to add image analysis
    to your applications. With Rekognition, you can detect objects, scenes, and faces
    in images. You can also search and compare faces. Rekognition&rsquo;s API enables
    you to quickly add sophisticated deep learning-based visual search and image classification
    to your applications.Amazon Rekognition is based on the same proven, highly scalable,
    deep learning technology developed by Amazon&rsquo;s computer vision scientists
    to analyze billions of images daily for Prime Photos. Amazon Rekognition uses
    deep neural network models to detect and label thousands of objects and scenes
    in your images, and we are continually adding new labels and facial recognition
    features to the service.Rekognition&rsquo;s API lets you easily build powerful
    visual search and discovery into your applications. With Amazon Rekognition, you
    only pay for the images you analyze and the face metadata you store. There are
    no minimum fees and there are no upfront commitments.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-rekognition.png
  humanURL: https://aws.amazon.com/rekognition/
  baseURL: :///
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/aws-rekognition/openapi.md
x-common:
- type: x-blog
  url: https://aws.amazon.com/rekognition/developers/#blog-posts
- type: x-customers
  url: https://aws.amazon.com/rekognition/customers/
- type: x-documentation
  url: http://docs.aws.amazon.com/rekognition/latest/dg/API_Reference.htm
- type: x-faq
  url: https://aws.amazon.com/rekognition/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/rekognition/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/rekognition/pricing/
- type: x-sdk
  url: https://aws.amazon.com/rekognition/developers/#sdk
- type: x-website
  url: https://aws.amazon.com/rekognition/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---