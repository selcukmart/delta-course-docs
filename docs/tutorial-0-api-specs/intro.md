---
sidebar_position: 1
---

# API Specifications

API is based on OpenAPI v3.

Every request **MUST** return `state` key. And if `state` is `"true"`, result is **true**.

Example:
```
{
    "state": "true",
    "data": {
        ...
    }
}
```
Every false result **MUST** return an `error` according to [https://datatracker.ietf.org/doc/html/rfc6749#section-4.1.2.1](https://datatracker.ietf.org/doc/html/rfc6749#section-4.1.2.1)

And lots of times return an `error_description` which explains the error reason.
```
{
    "state": "false",
    "error": "invalid_request"
}
```

## Where are `Login Credentials`

Username and passwords are defined in `users`. User type **MUST** be `API user`.

**_For Example:_**

It can be found on the menu `Users` in `Delta Course Automation Admin Panel`. User created by panel credentials are user's `API credentials`.

Credentials are only **username** and **password** as `user` and `secret`
