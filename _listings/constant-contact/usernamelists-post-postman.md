{
  "info": {
    "name": "Constant Contact Add Mailing List",
    "_postman_id": "551fd88e-2901-4e5d-a3ed-43cd9d224854",
    "description": "Add Mailing List",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mailing",
      "item": [
        {
          "id": "b3384f93-4fd2-4705-89c7-b83e93b47a8b",
          "name": "get-all-mailing-lists",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/lists"
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
            "description": "Get All Mailing Lists"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2dbbfe8d-0f8b-4890-b5d9-bc6277e8d9e9"
            }
          ]
        },
        {
          "id": "62cd0b55-b0ff-490f-a405-eb3c54d19db6",
          "name": "add-mailing-list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/lists"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add Mailing List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5341da1e-b1e8-4b4e-8f58-2f348312e494"
            }
          ]
        }
      ]
    }
  ]
}