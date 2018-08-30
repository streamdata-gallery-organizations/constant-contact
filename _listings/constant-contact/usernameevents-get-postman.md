{
  "info": {
    "name": "Constant Contact List Events",
    "_postman_id": "781f60a7-77df-467d-83db-c8aae176dbd0",
    "description": "List Events",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaign",
      "item": [
        {
          "id": "08a30f08-e535-47f2-a76c-aecff9a5cade",
          "name": "get-campaign-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/campaigns/:campaign-id/events/"
              ],
              "variable": [
                {
                  "id": "campaign-id",
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
            "description": "Get Campaign Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5efb1b5c-ce55-4bae-baa7-ca7f70fa63a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Per-Contact",
      "item": [
        {
          "id": "f1314a3e-413a-4443-80f5-f904e1f9f1c6",
          "name": "get-percontact-campaign-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts/:contact-id/events/"
              ],
              "variable": [
                {
                  "id": "contact-id",
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
            "description": "Get Per-Contact Campaign Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a390fbe7-4662-48c1-94c2-8d59890192ed"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "3bac7fd1-58f6-44e2-8684-3ad45ec695fd",
          "name": "list-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/events"
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
            "description": "List Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dec0950f-2ca9-425e-90dd-270d17358349"
            }
          ]
        }
      ]
    }
  ]
}