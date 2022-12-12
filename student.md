# Hapara Student Extension Docs

## Get Student Configuration
Make a request that is similar to the following:
```http
POST https://api.hapara.com/admin/config/highlights
Content-type: application/json

{
    "emails": ["schoolemail@yourschool.edu"],
    "flags": []
}
```
You should get a response like this
```http
HTTP 1.1 200 OK
Content-type: application/json
Access-control-allow-origin: *
access-control-expose-headers: Content-length

[
    
]
