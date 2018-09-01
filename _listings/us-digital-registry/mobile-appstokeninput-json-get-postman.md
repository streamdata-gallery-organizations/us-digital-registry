{
  "info": {
    "name": "U.S. Digital Registry Mobile App API Mobile App Token",
    "_postman_id": "d004037e-9438-43b7-a5d4-4d1dcd6d6e8d",
    "description": "This returns tokens representing agencies, tags, and a basic text search token for the purpose of building search dialogs",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mobile Apps",
      "item": [
        {
          "id": "41b33f2f-2fb0-41de-bdee-d5b9e88e5ca4",
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
              "id": "f2d67b23-84b8-4803-9800-6346649b1187"
            }
          ]
        }
      ]
    }
  ]
}