---
sidebar_position: 2
---

# Login

Login credentials can be taken from Admin Panel as a user. 

**_POSTMAN DOC URL;_**

[https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-d5195b3b-864a-4124-95e7-3795149c218c](https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-d5195b3b-864a-4124-95e7-3795149c218c)

### Request

**_Path;_**

`/api/o-auth2/login`

**_Method: POST_**

Credentials are: `user` and `secret`

### Response

**_Logged in;_**
```json
{
"state": "true",
"bearer": "AB1bl7iPaeN7fSUD94b48a00iN1Fq7H9uZkOkE94b48a00EqBY33d2M8xVl7nFEM8JXoapsV37e15"
}
```

**~~invalid_client~~**
```json
{
  "state": "false",
  "error_description": "User is not registered\n",
  "error": "invalid_client",
  "error_uri": "/api/o-auth2/login"
}
```

## TOKEN

Token expires at the end of the 2 hours.

## Code Examples

It can be taken from: [https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-d5195b3b-864a-4124-95e7-3795149c218c?ctx=code](https://www.postman.com/onlinekurum/workspace/delta-course-automation/request/3724027-d5195b3b-864a-4124-95e7-3795149c218c?ctx=code)