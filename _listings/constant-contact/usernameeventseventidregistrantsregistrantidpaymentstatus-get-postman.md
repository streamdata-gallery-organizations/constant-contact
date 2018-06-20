{
  "info": {
    "name": "Constant Contact Get Payment Status",
    "_postman_id": "e155b79c-deed-4e81-b63d-fddf5c01e672",
    "description": "Get Payment Status",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Payment",
      "item": [
        {
          "id": "f630a70d-770a-40f0-a272-07a9a845ae25",
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
              "id": "7a3db202-d664-49aa-b9eb-1d705761616f"
            }
          ]
        }
      ]
    }
  ]
}