{
  "info": {
    "name": "Kentico Cloud Retrieving visitor's segments",
    "_postman_id": "1e803edd-90d0-4290-be9d-a9162b304ac5",
    "description": "Use the Personalization API to retrieve the list of segments that the specified visitor belongs to.\n\n* Authenticate the request using your Personalization API Key.\n* Specify the User ID of the visitor you are asking about.\n \nSee <https://developer.kenticocloud.com/docs/personalizing-content#section-retrieving-visitor-s-segments> for more details.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "44704c41-4be1-4726-9be8-ee4026b94dac",
          "name": "Segment569030c752a544f5A243C5285b3eb24eVisitorsBySegmentNameGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "deliver.kenticocloud.com",
              "path": [
                "segment/569030c7-52a5-44f5-a243-c5285b3eb24e/:SegmentName/visitors"
              ],
              "variable": [
                {
                  "id": "SegmentName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve visitors that match the specified segment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1793360-310a-4534-911c-c3463d4e6f37"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieving",
      "item": [
        {
          "id": "ec085f87-9972-4f67-a6da-e72a4554417c",
          "name": "Visitor569030c752a544f5A243C5285b3eb24eE3e9e191a12b9257SegmentGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/e3e9e191a12b9257/segment",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Use the Personalization API to retrieve the list of segments that the specified visitor belongs to.\n\n* Authenticate the request using your Personalization API Key.\n* Specify the User ID of the visitor you are asking about.\n \nSee <https://developer.kenticocloud.com/docs/personalizing-content#section-retrieving-visitor-s-segments> for more details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "06f18d1d-8364-4726-a194-c5eec7f17e0b"
            }
          ]
        }
      ]
    }
  ]
}