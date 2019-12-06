# cURL requests to configure Google Analytics


Requirements:
**Workspace slug & Access token**


## Google Analytics
```
curl -X POST \
  https://platform.segmentapis.com/v1beta/workspaces/{{insert workspace slug here}}/sources/workshop_source/destinations/ \
  -H 'Authorization: Bearer {{insert access token here}}' \
  -H 'Content-Type: application/json' \
  -d '{
    "destination": {
      "name": "workspaces/{{insert workspace slug here}}/sources/workshop_source/destinations/google-analytics",
      "config": [
        {
          "name": "workspaces/{{insert workspace slug here}}/sources/workshop_source/destinations/google-analytics/config/trackingId",
          "type": "string",
          "value": UA-153856743-2
        }
      ],
      "enabled": false,
      "connection_mode": "CLOUD"
    }
  }
'
```

## Braze
```
curl -X POST \
  'https://platform.segmentapis.com/v1beta/workspaces/{{workspace_slug}}/sources/workshop_source/destinations/' \
  -H 'Accept: */*' \
  -H 'Authorization: Bearer {{insert access token here}}' \
  -H 'Content-Type: application/json' \
  -H 'Host: platform.segmentapis.com' \
  -d '{
    "destination": {
      "name": "workspaces/{{workspace_slug}}/sources/workshop_source/destinations/appboy",
      "config": [
        {
          "name": "workspaces/{{workspace_slug}}/sources/workshop_source/destinations/appboy/config/datacenter",
          "type": "string",
          "value": "us03"
        },
		 {
          "name": "workspaces/{{workspace_slug}}/sources/workshop_source/destinations/appboy/config/apiKey",
          "type": "string",
          "value": "35707c69-bf09-4821-8ae3-a514d5800ac9"
        }
        
      ],
      "enabled": false
    }
  }
'
```