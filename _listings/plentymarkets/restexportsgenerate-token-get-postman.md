{
  "info": {
    "name": "Plentymarkets Generate a token",
    "_postman_id": "df445ffe-c580-4355-9e5a-4d4690405e9f",
    "description": "Creates a new token which can be used as <code>OutputParam</code> entry.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Generate",
      "item": [
        {
          "id": "cf3ed42d-2fb5-48fc-8930-63369952ce34",
          "name": "getRestExportsGenerateToken",
          "request": {
            "url": "http://example.com/rest/exports/generate_token",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new token which can be used as <code>OutputParam</code> entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f085869-4486-44c8-80db-30a326215f70"
            }
          ]
        },
        {
          "id": "c1fcd56c-be15-450f-bc71-c994b5fdddda",
          "name": "postRestWarehousesLocationsPreviews",
          "request": {
            "url": "http://example.com/rest/warehouses/locations/previews",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Generates warehouse location preview and saves it"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40ec7d64-3100-4eaf-99db-5a43821808c6"
            }
          ]
        },
        {
          "id": "b75d9dac-0cab-4430-8b55-1136a748e8e7",
          "name": "getRestWarehousesLocationsWarehouseLabel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/warehouses/locations/:warehouseId/label"
              ],
              "variable": [
                {
                  "id": "warehouseId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Generates the warehouse location label"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d65f40e-c9eb-422d-9f33-5620caf598e6"
            }
          ]
        }
      ]
    }
  ]
}