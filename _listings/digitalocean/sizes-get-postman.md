{
  "info": {
    "name": "Digital Ocean List all Sizes",
    "_postman_id": "755ce3ef-ef91-4f3e-a9c1-a0901d6a7b53",
    "description": "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe response will be a JSON object with a key called _sizes_.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "23421a4c-826f-4384-9d45-159f7e401619",
          "name": "SizesGet",
          "request": {
            "url": "http://example.com/sizes",
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
            "description": "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe response will be a JSON object with a key called _sizes_."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d99efdb7-2f43-472f-99b6-8bd14e780e8d"
            }
          ]
        }
      ]
    }
  ]
}