# Create User's Account


**URL** : `https://solve-captcha.herokuapp.com/balance`

**Method** : `GET`

**Headers constraints**

```json
{
    "authorization": "your api_key"
}
```

**Headers example** All fields must be sent.

```json
{
	  "authorization": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJJRCI6NDUwMDE2MzA0MTY1NDM3MDAsImlhdCI6MTYzMDQxNjU0M30.JhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9-jazgz5-aA"
}
```

## Success Response

**Code** : `200 OK`

**Content example**

```json
{
    "code": 200,
    "api_key": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJJRCI6NDUwMDE2MzA0MTY1NDM3MDAsImlhdCI6MTYzMDQxNjU0M30.JhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9-jazgz5-aA",
    "balance": {
      "value": 3.48
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