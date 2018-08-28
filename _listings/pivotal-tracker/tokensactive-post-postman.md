{
  "info": {
    "name": "Pivotal Tracker Post Tokens Active",
    "_postman_id": "94d56169-86c5-4845-b0d5-b17d79dcf570",
    "description": "Returns an API token associated with the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tokens",
      "item": [
        {
          "id": "5769a56c-4b7c-4cbe-80d4-fcd551f0533e",
          "name": "getTokensActive",
          "request": {
            "url": "http://www.pivotaltracker.com/services/v3/tokens/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an API token associated with the user. This method requires HTTP Basic authentication."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc03763f-fd38-4488-b20d-d6b1ba406b05"
            }
          ]
        },
        {
          "id": "80014683-1459-4082-b78a-0c5a7421a9cd",
          "name": "postTokensActive",
          "request": {
            "url": "http://www.pivotaltracker.com/services/v3/tokens/active?password=%7B%7D&username=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an API token associated with the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63b92d83-9347-4896-b82b-29b084edf9d3"
            }
          ]
        }
      ]
    }
  ]
}