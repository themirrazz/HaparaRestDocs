# Hapara Student Extension Docs

## Get Student Configuration
Make a request that is similar to the following:
```http
POST https://api.hapara.com/admin/config/highlights
Content-type: application/json

{
    "emails": ["schoolemail@yourschool.edu"],
    "flags": ["example-flag-1","example-flag-2"]
}
```
You should get a response like this
```http
HTTP 1.1 200 OK
Content-type: application/json
Access-control-allow-origin: *
access-control-expose-headers: Content-length

[
    "Classes": [
        "9d3a0aa3-3f53-453e-98a2-448716e5799a@yourschool.edu",
        "4273b6b8-4fbe-45d9-b340-7d12f88b1f15@yourschool.edu",
        "167766e0-3820-46fd-aa10-07e927a007dd@yourschool.edu",
        "1d955a4d-73af-40d6-864a-f96f720e3a92@yourschool.edu",
        "9977f190-1602-49de-94b1-72a710ca05b5@yourschool.edu",
        "cf95c1fc-24d1-480e-9ccb-15e1a3fc9817@yourschool.edu"
    ],
    "Email": "schoolemail@yourschool.edu",
    "FeatureFlags": {
        "example-flag-1": false,
        "example-flag-2": true
    },
    "ID": "553187120532800203556",
    "InvalidCode": "",
    "MonitoringTime": {
        "CurrentTime": "2022-1-1T09:07:13.30150255-6:00",
        "Saturday": false,
        "Sunday": false,
        "StartTime": "09:00",
        "EndTime":"16:00",
        "TimeZone":"America/Chicago"
    },
    "ScreenshotBusURL": "https://hl.hapara.com/oxygen-screens/watch/hl/student/",
    "ScreenshotsConfig": {
        ScreenshotsHiResHeight: 600,
        ScreenshotsHiResWidth: 800,
        ScreenshotsHiResQuality: 0.8,
        ScreenshotsLoResHeight: 300,
        ScreenshotsLoResWidth: 300,
        ScreenshotsLoResQuality: 0.3
    },
    "Valid": true,
    "WhiteList": [
        "^chrome://settings*",
        "^chrome://camera-app/*",
        "^chrome://file-manager*",
        "https://onlineclasswork.yourschool.edu/*"
    ],
    "PrimaryEmail": "schoolemail@yourschool.edu",
    "LogURL": ""
]
```
