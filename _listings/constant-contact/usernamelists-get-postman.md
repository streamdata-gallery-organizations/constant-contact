{
  "info": {
    "name": "Constant Contact Get All Mailing Lists",
    "_postman_id": "9d5121c3-3c7e-43c6-8900-8191b5854b1f",
    "description": "Get All Mailing Lists",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mailing",
      "item": [
        {
          "id": "1687a8b3-0bd4-4e80-91f3-0d4e9f14778b",
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
              "id": "cfa35421-86ec-499b-9930-3261fb11e353"
            }
          ]
        }
      ]
    }
  ]
}