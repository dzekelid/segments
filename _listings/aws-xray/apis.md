---
name: AWS X-Ray
x-slug: aws-xray
description: AWS X-Ray helps developers analyze and debug production, distributed
  applications, such as those built using a microservices architecture. With X-Ray,
  you can understand how your application and its underlying services are performing
  to identify and troubleshoot the root cause of performance issues and errors. X-Ray
  provides an end-to-end view of requests as they travel through your application,
  and shows a map of your applications underlying components. You can use X-Ray to
  analyze both applications in development and in production, from simple three-tier
  applications to complex microservices applications consisting of thousands of services.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-xray.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Segments
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/segments/master/_listings/aws-xray/apis.md
specificationVersion: "0.14"
apis:
- name: AWS X-Ray API Put Trace Segments
  x-api-slug: aws-xray-api
  description: Uploads segment documents to AWS X-Ray.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-xray.png
  humanURL: https://aws.amazon.com/xray/
  baseURL: ://///?Action=PutTraceSegments
  tags: Trace Segments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/segments/master/_listings/aws-xray/actionputtracesegments-get-openapi.md
- name: AWS X-Ray API
  x-api-slug: aws-xray-api
  description: AWS X-Ray helps developers analyze and debug production, distributed
    applications, such as those built using a microservices architecture. With X-Ray,
    you can understand how your application and its underlying services are performing
    to identify and troubleshoot the root cause of performance issues and errors.
    X-Ray provides an end-to-end view of requests as they travel through your application,
    and shows a map of your applications underlying components. You can use X-Ray
    to analyze both applications in development and in production, from simple three-tier
    applications to complex microservices applications consisting of thousands of
    services.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/aws-xray.png
  humanURL: https://aws.amazon.com/xray/
  baseURL: :///
  tags: Segments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/segments/master/_listings/aws-xray/openapi.md
x-common:
- type: x-documentation
  url: http://docs.aws.amazon.com/xray/latest/api/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/xray/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/xray/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/xray/pricing/
- type: x-website
  url: https://aws.amazon.com/xray/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---