{
  "info": {
    "name": "Digital Ocean List all certificates",
    "_postman_id": "874a0ab2-aed6-4ecc-b7bc-59710533feb0",
    "description": "To list all of the certificates available on your account, send a GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object with a certificates key. This will be set to an array of certificate objects, each of which will contain the standard certificate attributes:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "29bb54cf-bf5a-47b1-b9fa-b3a59339b90c",
          "name": "CertificatesGet",
          "request": {
            "url": "http://example.com/certificates",
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
            "description": "To list all of the certificates available on your account, send a GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object with a certificates key. This will be set to an array of certificate objects, each of which will contain the standard certificate attributes:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e6f5e4e-bc3d-4fb8-9416-c75267a96ef1"
            }
          ]
        }
      ]
    }
  ]
}