curl -X POST \
  https://platform.segmentapis.com/v1beta/workspaces/yanis_sandbox/sources/typewriter_demo/destinations/ \
  -H 'Authorization: Bearer DU9XEkxHmN7oOHF0OuW_vjv-0Ny0Zgw2nRZw-0P1f-U.ugkH2exch77Eqw8HD5KUjo0GF4y3NssFthQo0EJwZa0' \
  -H 'Content-Type: application/json' \
  -H 'Postman-Token: 25fc1f4d-b4fb-48cc-8a8f-abff884cdae3' \
  -H 'cache-control: no-cache' \
  -d '{
    "destination": {
      "name": "workspaces/yanis_sandbox/sources/typewriter_demo/destinations/google-analytics",
      "config": [
        {
          "name": "workspaces/yanis_sandbox/sources/typewriter_demo/destinations/google-analytics/config/trackingId",
          "type": "string",
          "value": UA-153856743-2
        }
      ],
      "enabled": false,
      "connection_mode": "CLOUD"
    }
  }
'