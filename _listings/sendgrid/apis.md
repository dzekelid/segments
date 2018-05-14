---
name: SendGrid
description: SendGrid is a cloud-based email service that delivers email on behalf
  of companies to increase deliverability and improve customer communications integration
  with new or existing email systems is done via SMTP or through a REST API, providing
  metrics on outgoing email, and handles unsubscribe links, abiding by anti-spam regulations.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/sendgrid-logo.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Stack
- Plans
- Partners
- Messaging
- Messaging
- Imports
- Email
- Email
- API LIfeycle
created: "2018-03-24"
modified: "2018-03-24"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/segments/master/_listings/sendgrid/apis.yaml
specificationVersion: "0.14"
apis:
- name: SendGrid
  description: SendGrid is a cloud-based email service that delivers email on behalf
    of companies to increase deliverability and improve customer communications integration
    with new or existing email systems is done via SMTP or through a REST API, providing
    metrics on outgoing email, and handles unsubscribe links, abiding by anti-spam
    regulations
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/sendgrid-logo.png
  humanURL: ""
  baseURL: https://api.sendgrid.com//v3
  tags: Segments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/segments/master/_listings/sendgrid/contactdb-segments-segment-id-recipients-get.md
- name: SendGrid Add Contactdb Segments
  description: "**This endpoint allows you to create a segment.**\n\nAll recipients
    in your contactdb will be added or removed automatically depending on whether
    they match the criteria for this segment.\n\nList Id:\n\n* Send this to segment
    from an existing list\n* Don't send this in order to segment from your entire
    contactdb.\n\nValid operators for create and update depend on the type of the
    field you are segmenting: \n\n* **Dates:** \"eq\", \"ne\", \"lt\" (before), \"gt\"
    (after) \n* **Text:** \"contains\", \"eq\" (is - matches the full field), \"ne\"
    (is not - matches any field where the entire field is not the condition value)
    \n* **Numbers:** \"eq\", \"lt\", \"gt\" \n* **Email Clicks and Opens:** \"eq\"
    (opened), \"ne\" (not opened) \n\nSegment conditions using \"eq\" or \"ne\" for
    email clicks and opens should provide a \"field\" of either *clicks.campaign_identifier*
    or *opens.campaign_identifier*. The condition value should be a string containing
    the id of a completed campaign. \n\nSegments may contain multiple condtions, joined
    by an \"and\" or \"or\" in the \"and_or\" field. The first condition in the conditions
    list must have an empty \"and_or\", and subsequent conditions must all specify
    an \"and_or\".\n\nThe Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
    recipients.\n\nFor more information about segments in Marketing Campaigns, please
    see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment)."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/sendgrid-logo.png
  humanURL: https://sendgrid.com/
  baseURL: https://api.sendgrid.com//v3
  tags: Segments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/segments/master/_listings/sendgrid/contactdb-segments-post.md
x-common:
- type: x-net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-nodejs-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: https://sendgrid.com/
- type: x-net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-nodejs-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---