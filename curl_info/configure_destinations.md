# cURL requests to configure Google Analytics & Braze


Requirements:
**Workspace slug & Access token**


## Google Analytics
```
curl -X POST \
  https://platform.segmentapis.com/v1beta/workspaces/{{workspace_slug}}/sources/workshop_source/destinations/ \
  -H 'Authorization: Bearer {{access_token}}' \
  -H 'Content-Type: application/json' \
  -d '{
    "destination": {
      "name": "workspaces/{{workspace_slug}}/sources/workshop_source/destinations/google-analytics",
      "config": [
        {
          "name": "workspaces/{{workspace_slug}}/sources/workshop_source/destinations/google-analytics/config/trackingId",
          "type": "string",
          "value": UA-153856743-2
        }
      ],
      "enabled": true,
      "connection_mode": "CLOUD"
    }
  }
'
```
