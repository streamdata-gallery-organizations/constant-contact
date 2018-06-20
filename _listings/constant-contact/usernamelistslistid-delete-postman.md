{
  "info": {
    "name": "Constant Contact Delete Mailing List",
    "_postman_id": "2792409e-4734-4506-8be8-b4088e0f951a",
    "description": "Delete Mailing List",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mailing",
      "item": [
        {
          "id": "87c16ebf-bc9c-4ea6-a557-79ca637cb115",
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
              "id": "b22616bd-8858-4f40-aa86-4d4bdac1ebaa"
            }
          ]
        },
        {
          "id": "70674348-7949-4e9a-b003-c690fa0d69b2",
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
              "id": "24d8fc0b-3b6d-4ccf-8a69-a6bd0c4f2087"
            }
          ]
        },
        {
          "id": "f8eec224-1c4a-400a-a0fa-d98d7b6a4f26",
          "name": "delete-mailing-list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/lists/:list-id"
              ],
              "variable": [
                {
                  "id": "list-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Mailing List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "799231d3-642a-4853-8fb4-de8ecb3179d3"
            }
          ]
        }
      ]
    }
  ]
}