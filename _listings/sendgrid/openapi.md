---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  description: the-sendgrid-web-api-v3-documentation--this-is-the-entirety-of-the-documented-v3-endpoints--we-have-updated-all-the-descriptions-parameters-requests-and-responses--authentication-every-endpoint-requires-authentication-in-the-form-of-an-authorization-header-authorization-bearer-api-key
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contactdb/segments:
    get:
      summary: Get Contactdb Segments
      description: |-
        **This endpoint allows you to retrieve all of your segments.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.get
      x-api-path-slug: contactdbsegments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
    post:
      summary: Add Contactdb Segments
      description: "**This endpoint allows you to create a segment.**\n\nAll recipients
        in your contactdb will be added or removed automatically depending on whether
        they match the criteria for this segment.\n\nList Id:\n\n* Send this to segment
        from an existing list\n* Don't send this in order to segment from your entire
        contactdb.\n\nValid operators for create and update depend on the type of
        the field you are segmenting: \n\n* **Dates:** \"eq\", \"ne\", \"lt\" (before),
        \"gt\" (after) \n* **Text:** \"contains\", \"eq\" (is - matches the full field),
        \"ne\" (is not - matches any field where the entire field is not the condition
        value) \n* **Numbers:** \"eq\", \"lt\", \"gt\" \n* **Email Clicks and Opens:**
        \"eq\" (opened), \"ne\" (not opened) \n\nSegment conditions using \"eq\" or
        \"ne\" for email clicks and opens should provide a \"field\" of either *clicks.campaign_identifier*
        or *opens.campaign_identifier*. The condition value should be a string containing
        the id of a completed campaign. \n\nSegments may contain multiple condtions,
        joined by an \"and\" or \"or\" in the \"and_or\" field. The first condition
        in the conditions list must have an empty \"and_or\", and subsequent conditions
        must all specify an \"and_or\".\n\nThe Contacts API helps you manage your
        [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
        recipients.\n\nFor more information about segments in Marketing Campaigns,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment)."
      operationId: contactdb.segments.post
      x-api-path-slug: contactdbsegments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
  /contactdb/segments/{segment_id}:
    delete:
      summary: Delete Contactdb Segments Segment
      description: |-
        **This endpoint allows you to delete a segment from your recipients database.**

        You also have the option to delete all the contacts from your Marketing Campaigns recipient database who were in this segment.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.segment_id.delete
      x-api-path-slug: contactdbsegmentssegment-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: delete_contacts
        description: True to delete all contacts matching the segment in addition
          to deleting the segment
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
      - Segment
    get:
      summary: Get Contactdb Segments Segment
      description: |-
        **This endpoint allows you to retrieve a single segment with the given ID.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.segment_id.get
      x-api-path-slug: contactdbsegmentssegment-id-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: segment_id
        description: The ID of the segment you want to request
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
      - Segment
    patch:
      summary: Patch Contactdb Segments Segment
      description: |-
        **This endpoint allows you to update a segment.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.segment_id.patch
      x-api-path-slug: contactdbsegmentssegment-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: segment_id
        description: The ID of the segment you are updating
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
      - Segment
  /contactdb/segments/{segment_id}/recipients:
    get:
      summary: Get Contactdb Segments Segment  Recipients
      description: |-
        **This endpoint allows you to retrieve all of the recipients in a segment with the given ID.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.segment_id.recipients.get
      x-api-path-slug: contactdbsegmentssegment-idrecipients-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: page
      - in: query
        name: page_size
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
      - Segment
      - ""
      - Recipients
---