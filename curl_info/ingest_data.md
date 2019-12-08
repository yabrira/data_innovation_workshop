# cURL requests to ingest data

Requirements:
**Base64 encoded write key**

## Identify

```
curl -X POST \
  https://api.segment.io/v1/identify \
  -H 'Accept: application/json' \
  -H 'Authorization: Basic {{segment_write_key}}' \
  -H 'Content-Type: application/json' \
  -d '{
    "userId": "api_workshop_user"
}'
```

## Track

```
curl -X POST \
  https://api.segment.io/v1/track \
  -H 'Accept: application/json' \
  -H 'Authorization: Basic {{segment_write_key}}' \
  -H 'Content-Type: application/json' \
  -d '{
    "userId": "api_workshop_user",
    "event": "Event sent"
}'
```

## Page

```
curl -X POST \
  https://api.segment.io/v1/page \
  -H 'Accept: application/json' \
  -H 'Authorization: Basic {{segment_write_key}}' \
  -H 'Content-Type: application/json' \
  -d '{
    "userId": "api_workshop_user",
    "name": "home_page"
}'
```

## Batch

```
curl -X POST \
  https://api.segment.io/v1/batch \
  -H 'Accept: application/json' \
  -H 'Content-Type: application/json' \
  -H 'Authorization: Basic {{segment_write_key}}' \
  -d '{
    "batch": [{
            "type": "identify",
            "userId": "api_master"
        },
        {
            "type": "identify",
            "userId": "api_student"
        },
        {
            "type": "track",    
            "userId": "api_master",
            "event": "APIs Mastered",
            "properties": {
                "api": 1
            }
        },
        {
            "type": "track",
            "userId": "api_student",
            "event": "APIs Studied",
            "properties": {
                "api": 1
            }
        },
        {
            "type": "track",
            "userId": "api_master",
            "event": "APIs Mastered",
            "properties": {
                "api": 2
            }
        },
        {
            "type": "track",
            "userId": "api_student",
            "event": "APIs Studied",
            "properties": {
                "api": 2
            }
        },
        {
            "type": "track",
            "userId": "api_master",
            "event": "APIs Mastered",
            "properties": {
                "api": 3
            }
        },
        {
            "type": "track",
            "userId": "api_student",
            "event": "APIs Studied",
            "properties": {
                "api": 3
            }
        },
        {
            "type": "track",
            "userId": "api_master",
            "event": "APIs Mastered",
            "properties": {
                "api": 4
            }
        },
        {
            "type": "track",
            "userId": "api_student",
            "event": "APIs Studied",
            "properties": {
                "api": 4
            }
        },
        {
            "type": "page",
            "userId": "api_student",
            "properties": {
                "name": "Home"
            }
        }, 
        {
            "type": "page",
            "userId": "api_master",
            "properties": {
                "name": "Home"
            }
        },
        {
            "type": "page",
            "userId": "api_student",
            "properties": {
                "name": "Paris"
            }
        }, 
        {
            "type": "page",
            "userId": "api_master",
            "properties": {
                "name": "Paris"
            }
        }  

    ]
}
```
