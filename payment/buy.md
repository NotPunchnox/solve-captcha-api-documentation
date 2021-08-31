# Create User's Account


**URL** : `https://solve-captcha.herokuapp.com/payment`

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
    "price": "[number 3 min]"
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
    "price": 3.002
}
```

## Success Response

**Code** : `201 CREATED`

**Content example**

```json
{
    "code": 201,
    "message": {
      "link": "https://www.sandbox.paypal.com/cgi-bin/webscr?cmd=_express-checkout&token=EZ56EAZ5E4AE-54AZ"
    }
}
```

**/!\\** : `Find the link and follow the instructions, ( paypal secure link )`

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
    "message": "Please specify a price"
}
```