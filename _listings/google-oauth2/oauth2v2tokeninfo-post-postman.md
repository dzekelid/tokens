{
  "info": {
    "name": "Google OAuth2 APIs Get Token Info",
    "_postman_id": "5c37129b-69b0-4825-a897-2843695c7bb9",
    "description": "Get the token information for this session.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Certificate",
      "item": [
        {
          "id": "3493d8a4-338c-435c-922d-ae59b055dbe1",
          "name": "oauth2.getCertForOpenIdConnect",
          "request": {
            "url": "http://www.googleapis.com/oauth2/v2/certs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the certification for this session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4d4a7c7-1826-4e36-89a1-60db9d7199d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Token",
      "item": [
        {
          "id": "16472a2d-b796-4f44-a910-bc4aaa94766d",
          "name": "oauth2.tokeninfo",
          "request": {
            "url": "http://www.googleapis.com/oauth2/v2/tokeninfo?access_token=%7B%7D&id_token=%7B%7D&token_handle=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Get the token information for this session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "784bba38-2a89-4b42-a824-58be0498a71d"
            }
          ]
        }
      ]
    }
  ]
}