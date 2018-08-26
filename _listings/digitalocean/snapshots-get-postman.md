{
  "info": {
    "name": "Digital Ocean List all Volume snapshots",
    "_postman_id": "4acb037d-182c-4707-8b84-172224d22029",
    "description": "To retrieve only snapshots based on volumes, include the resource_type query paramter set to volume, /v2/snapshots?resource_type=volume.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "48625f07-92b6-4a50-9cfa-02cae9646063",
          "name": "SnapshotsGet3",
          "request": {
            "url": "http://example.com/snapshots?page=%7B%7D&per_page=%7B%7D&resource_type=%7B%7D",
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
            "description": "To retrieve only snapshots based on volumes, include the resource_type query paramter set to volume, /v2/snapshots?resource_type=volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3ded6b3-cf35-4937-aabd-0188de1e1ffd"
            }
          ]
        }
      ]
    }
  ]
}