{
  "info": {
    "name": "U.S. Digital Registry Mobile App API Mobile Apps",
    "_postman_id": "7453252a-7528-4724-8b2d-1881305aebb6",
    "description": "This lists all active mobile apps.  It accepts parameters to perform basic search as well as searching by tag and agency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mobile Apps",
      "item": [
        {
          "id": "01aba94f-cb25-427e-ae7a-f7e53df41ab1",
          "name": "Api::V1::MobileApps#tokeninput",
          "request": {
            "url": "http://usdigitalregistry.digitalgov.gov/api/v1/mobile_apps/tokeninput.json?q=%7B%7D",
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
            "description": "This returns tokens representing agencies, tags, and a basic text search token for the purpose of building search dialogs"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4243836a-2bd5-4846-a9d3-a61ec947cdf9"
            }
          ]
        },
        {
          "id": "cd9fbd5c-3cae-4643-8b42-e4e4c3750d32",
          "name": "Api::V1::MobileApps#index",
          "request": {
            "url": "http://usdigitalregistry.digitalgov.gov/api/v1/mobile_apps.json?agencies=%7B%7D&language=%7B%7D&page=%7B%7D&page_size=%7B%7D&q=%7B%7D&tags=%7B%7D",
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
            "description": "This lists all active mobile apps.  It accepts parameters to perform basic search as well as searching by tag and agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13700c2d-c75b-4e3c-9802-e94513ed358c"
            }
          ]
        }
      ]
    }
  ]
}