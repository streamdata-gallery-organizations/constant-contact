{
  "info": {
    "name": "Constant Contact List Folders",
    "_postman_id": "ba0417be-985a-445b-b19b-471fef65a8a3",
    "description": "List Folders",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "5ba3a322-5674-4e4f-a59c-d1f360282722",
          "name": "list-folders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/library/folders"
              ],
              "query": [
                {
                  "key": "Accept",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Folders"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d734f40c-ead4-48b3-8b9e-2c575984e1f2"
            }
          ]
        }
      ]
    }
  ]
}