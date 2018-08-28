swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 1
info:
  title: Kentico Cloud
  description: this-is-a-collection-of-resources-you-can-find-within-the-kentico-cloud-developer-hubhttpsdeveloper-kenticocloud-com--kentico-cloudhttpskenticocloud-com-is-a-cloudfirst-headless-cms-that-allows-you-to-distribute-content-to-any-channel-and-device-websites-mobile-devices-mixed-reality-devices-presentation-kiosks-etc--through-an-api-certain-apis-require-that-you-include-the-authorization-header--find-more-in-httpsdeveloper-kenticocloud-comreferenceauthentication-
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/7888c9a3824a11f1/segments:
    get:
      summary: List segments of a visitor
      description: Retrieve the names of segments that the specified visitor belongs
        to.
      operationId: Visitor569030c752a544f5A243C5285b3eb24e7888c9a3824a11f1SegmentsGet
      x-api-path-slug: visitor569030c752a544f5a243c5285b3eb24e7888c9a3824a11f1segments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Segments
      - Of
      - Visitor
  /visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/e3e9e191a12b9257/segment:
    get:
      summary: Retrieving visitor's segments
      description: "Use the Personalization API to retrieve the list of segments that
        the specified visitor belongs to.\n\n* Authenticate the request using your
        Personalization API Key.\n* Specify the User ID of the visitor you are asking
        about.\n \nSee <https://developer.kenticocloud.com/docs/personalizing-content#section-retrieving-visitor-s-segments>
        for more details."
      operationId: Visitor569030c752a544f5A243C5285b3eb24eE3e9e191a12b9257SegmentGet
      x-api-path-slug: visitor569030c752a544f5a243c5285b3eb24ee3e9e191a12b9257segment-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieving
      - Visitors
      - Segments
  /segment/569030c7-52a5-44f5-a243-c5285b3eb24e/{SegmentName}/visitors:
    get:
      summary: List visitors of a segment
      description: Retrieve visitors that match the specified segment.
      operationId: Segment569030c752a544f5A243C5285b3eb24eVisitorsBySegmentNameGet
      x-api-path-slug: segment569030c752a544f5a243c5285b3eb24esegmentnamevisitors-get
      parameters:
      - in: path
        name: SegmentName
      responses:
        200:
          description: OK
      tags:
      - List
      - Visitors
      - Of
      - Segment