{
  "info": {
    "name": "Constant Contact Update Mailing List",
    "_postman_id": "1f951d74-7cbf-4bbf-ac96-e341276fb76c",
    "description": "Update Mailing List",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mailing",
      "item": [
        {
          "id": "09e32fc5-e3fb-4bbb-9515-b2c8d60c2df0",
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
              "id": "e9dde97b-dc2d-4ef0-a107-99805e08dbee"
            }
          ]
        },
        {
          "id": "c7070896-4d77-4ac6-b408-b3c09712309c",
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
              "id": "75cd54c6-30b9-4691-80fd-2ae838b60de1"
            }
          ]
        },
        {
          "id": "3f10f099-2778-44cf-b989-8caa13c27834",
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
              "id": "809eaa67-5cc4-4b82-855f-868bb782be80"
            }
          ]
        },
        {
          "id": "1cd03a75-5045-4121-8519-3d0a9813bf2f",
          "name": "update-mailing-list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/lists/:list-id"
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update Mailing List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "401a2f96-a8d4-47e8-a53c-52b52b997a9a"
            }
          ]
        },
        {
          "id": "7fe518d2-a175-401d-8768-7371f8dec7ff",
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
              "id": "39ce6482-1f0c-47b3-854f-370b975956e6"
            }
          ]
        }
      ]
    }
  ]
}