# Create User's Account


**URL** : `https://solve-captcha.herokuapp.com/solve`

**Method** : `POST`

**Headers constraints**

```json
{
    "authorization": "your api_key"
}
```

**Data constraints**

```json
{
	  "sitekey": "uuid",
	  "host": "url"
}
```

**Headers example** All fields must be sent.

```json
{
	  "authorization": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJJRCI6NDUwMDE2MzA0MTY1NDM3MDAsImlhdCI6MTYzMDQxNjU0M30.JhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9-jazgz5-aA"
}
```
**Data example**

```json
{
	  "sitekey": "f5561ba9-8f1e-40ca-9b5b-a0b3f719ef34",
	  "host": "https://discord.com/register"
}
```

## Success Response

**Code** : `200 OK`

**Content example**

```json
{
  "code": 200,
    "message": {
      "key": "P0_eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJwYXNza2V5IjoiR1h2azdOMlZtWTJFTTliajg4dlh2cHFVUVFPS0VYa3ZoaWtWYzc3NXl5QTd1U0Y3T0h5ay80NzM4eXNPOXQvSVlKVG4rbDlJRmVQS2lLbGkxQjlqVU4xRXhTVFM3RWJMaXo1SWxQRTN2WVpaVVBCMlQvemFjclRlU1o4c2JOODQ4R3J1K1F0eFJnaTQ4bmcxL0JXUnU3S2lTTnlYTDVWR2VYeUNacXNXdk1VYnZyK3I5WlR2blo5SmdINXZwUHRNUHRMM2lvU1hJczBWWitaOExuV1lyZjl3cnVkSGZZSGhvVkNEUG5vQi9Ba3NOV0FHVXZOTU16aWoyVktTV1RZT2dWVExiOXBuTVZJblNZSjNRTkJIWUtHSHJ2QkJPZGd4WWhENkNZZFB3bVcxV3kvUXZHdExqb0xnYnQydzY0SXpOMys2NFVpNFFubVdKbTZKd0ZJWmM2Ukk5NDNsUTZwR0RRQ0ZPa2ZseUU5dG9CZVBtS0I3aTZTR3FMeUlUYk03c1hydW0wUkxkNFh1ZnJIMGZ0aW5zSlN2bmxPSk5YWnM2MzAydnp6eDRWNkhCcUZKUm1SUkt3R21QcW41eFg4NlFtSEZsSG5sdE5iQ0lWVE8wYnZJcmRPbU55OVdLZlNDU2tEb0krVkYrdExaRU1keVpSWno3TGg0Tk5GUjFMSXpUSXVtSVgvd1RJR3pwYm8rc1A4SHA2VzZOalVSVk5zNjhHakdMcTcrOUExK1RJOVdZa2dhcXpSdkc3Q2VLUE9wZmZCb3VGVUNpQ2N3VERoNWIyNTNLNEVXclBvSGRja1Z5NHRMNjdGL2RuekJFcHpwZjdFNFhtL3d4eDBlUXowUllvZVFITVBtWnY0WnZPMytGRDZVdTR5b3lmdVhxM0hSZ0Jpbmx5TWVYcHQrekU2Zk9XUGZINjZJSFU1RnA0YTZJY3VNVFBma1IzdDhaUy9aMGpCNmQ1aEZOV1FKVkk3TTJIRnFobGxpaEtlZVRJejRybHBjV2tsaW9oMHlwWmxOd0cxOTJCQU9lWDdaUUY0NkpDY0tsc09RelI5RlVWcUp4WitIZWxLVWRkVUFhellPZC9qekR5Y202M24xRG9HUFpVV3J3NHFLVHhQOGdwTVIwbm95eTBpbFgvNDB1K3YyUmNxZmNxM0pyMHVkNS9BMU9aMytwMGZSaHQrWll1NFdxRFBQb2NhaDFBdFNnRlJXNFdFdE5rTDlGeGtaUUZodFFockJzT2E1SzA0c2ZVbmh0Q2R5UnRXZVZJNUc3ZmVZd0hYMVFNd0xsL0pVRUczZ2xRUGpMVWpHRzF2eUk2V3ZJWHhlZXZkUkdqVU1TcytwcHc5Y2RrK0FZYTEvY0hnWjRtMHBBZjZUQ2JKQksrTEtxVW5BWk53TXJsc2hQbGNsYlo5d3I3b0VZWlFKd0xzdlRuNUVxQmgwSzNCTGEwdDJnOXlXdHpoS2UrVVZ3djZrWk5FY29kQWdZSmpqZFhqR082SGdDRUlLVkFDaDhRWmJ5clZodjJMVE0yaUNlSUxJMHRDOUFidk1lS2w0NFNxL1QvN0s4UHVoYU1nQjB4cjEyT1pFbXA1TXg0bENLcDZvbmJOdGtVQTAvL2VoMHg0SEhSTG9EUEtLaFMrZzErUU9NRldKZHJHbkgwUlZ0UEFaUzgzNmdLNVRDaVhJTFE5cnhlemZyMkFrZlhXR2Fuc01YMDZBUXYxYXh1RDRyN3NyckRRQVM3akdCVUxLK21LUGN5SXB2dEFSMmNZdERRbmpIck9tUFlOSGRDaG1XZFhzQXI3bGluNDI3L0xFV3kwNnVSOUorRG1pSkM3U2ZYSjUvaE9BWGdhQnJNR2Q2OXpqcnoyMUEwSUlJdlRCdTZxYjBNWXFnZjdLUlQrNy9ZWVF6SEw2NDkzN2ZwRS9lSEwxTUZHeURhYVpxYkhyQTZ6ZnJYUTNkU1pSN3B0V3hud0w2QT09Njg2RUdJMDJMTUFtMy9aVSIsImV4cCI6MTYzMDQyMzYxNiwic2hhcmRfaWQiOjUzNTc2NTU5LCJwZCI6MH0.0oSZi5A67w63sRcCzFO0P_GDl2JDza8WRmDCQonrsGE",
      "client": {
        "api_key": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJJRCI6NDUwMDE2MzA0MTY1NDM3MDAsImlhdCI6MTYzMDQxNjU0M30.JhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9-jazgz5-aA",
        "price": 0.002,
        "balance": 3.488
      }
    }
}
```

## Error Responses

**Condition** : If api_key Not exist.

**Code** : `401 UNAUTHORIZED`

**Content example** : 

```json
{
    "code": 404,
    "message": "unauthorized"
}
```

### Or

**Condition** : If fields are missed.

**Code** : `400 BAD REQUEST`

**Content example**

```json
{
    "code": 400,
    "message": "Please specify sitekey or host"
}
```