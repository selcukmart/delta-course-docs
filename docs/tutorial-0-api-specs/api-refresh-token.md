---
sidebar_position: 3
---

# Refresh Token

Expire time is 7200 second.

You MUST refresh token before expire time.

**_POSTMAN DOC URL;_**

[https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-37776a8f-c27a-4a06-b0c0-2fbef1fc2b52)

### Request

**_Path;_**

`/api/o-auth2/refresh-token`

**_Method: POST_**

Credentials is: `refresh_token`

### Response

**_Logged in;_**
```json
{
  "state": "true",
  "bearer": "fb6f196e9e17d2b756cae6d63fae3394",
  "refresh_token": "ac388e0e42589faee4e80f84461f495f",
  "expires": 7200
}
```

**~~invalid_client~~**
```json
{
  "state": "false",
  "error_description": "User is not registered\n",
  "error": "invalid_client",
  "error_uri": "/api/o-auth2/refresh-token"
}
```

## TOKEN

Token expires at the end of the 2 hours.

## Code Examples

It can be taken from: [https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-37776a8f-c27a-4a06-b0c0-2fbef1fc2b52?ctx=code)