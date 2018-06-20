{
  "info": {
    "name": "Constant Contact Update Payment Status",
    "_postman_id": "3a7dde5d-497c-4be3-8759-19e610f14c04",
    "description": "Update Payment Status",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Payment",
      "item": [
        {
          "id": "4f0b5e02-e268-4395-afa2-17cbd6893de9",
          "name": "get-payment-status",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/events/:event-id/registrants/:registrant-id/paymentstatus"
              ],
              "variable": [
                {
                  "id": "event-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "registrant-id",
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
            "description": "Get Payment Status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9e625b3-ac39-4441-b76c-9ae420e13b01"
            }
          ]
        },
        {
          "id": "87d89642-c1f8-4541-bfab-496646d1f9b8",
          "name": "update-payment-status",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/events/:event-id/registrants/:registrant-id/paymentstatus"
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
                  "id": "event-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "registrant-id",
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
            "description": "Update Payment Status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8e42b3c-9ff1-456d-9d76-ca7d7956e8d6"
            }
          ]
        }
      ]
    }
  ]
}