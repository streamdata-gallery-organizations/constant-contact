{
  "info": {
    "name": "Constant Contact List Activities",
    "_postman_id": "e713cdfa-9dcf-4e42-9a87-9364cd5510b7",
    "description": "List Activities",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "50f72e62-65a8-443d-866a-c629fdb88053",
          "name": "list-activities",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/activities"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Activities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3c4e04c-03e8-4cb0-a90b-80e5e7bac1eb"
            }
          ]
        }
      ]
    }
  ]
}