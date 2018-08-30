{
  "info": {
    "name": "Constant Contact Get Mailing List",
    "_postman_id": "afa12858-8606-470b-925d-20e9b99753bf",
    "description": "Get Mailing List",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mailing",
      "item": [
        {
          "id": "a24628da-7023-4064-a583-7b20045867f2",
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
              "id": "8768356a-5beb-43aa-9ae8-0696a9094976"
            }
          ]
        },
        {
          "id": "cc52db0e-07cc-436b-af74-c27e5c831649",
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
              "id": "eeed6775-f789-40a9-9329-0b797acc21d2"
            }
          ]
        },
        {
          "id": "dd3ac185-4ea8-4ddc-8926-07e101d87e10",
          "name": "get-mailing-list",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Mailing List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e59f038d-4337-4d52-8b30-ffbab32b977b"
            }
          ]
        },
        {
          "id": "bc85f7e4-e6ba-40d7-9d2a-910c919297f3",
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
              "id": "9a45e7e4-ce0a-4a58-9ef1-72ee75fc1bcb"
            }
          ]
        }
      ]
    }
  ]
}