# Create User's Account


**URL** : `https://solve-captcha.herokuapp.com/auth/login/`

**Method** : `POST`

**Data constraints**

```json
{
    "email": "your email",
    "password": "your password"
}
```

**Data example** All fields must be sent.

```json
{
	  "email": "name@example.com",
	  "password": "my_password"
}
```

## Success Response

**Code** : `200 OK`

**Content example**

```json
{
    "code": 200,
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJJRCI6NDUwMDE2MzA0MTY1NDM3MDAsImlhdCI6MTYzMDQxNjU0M30.JhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9-jazgz5-aA"
}
```

## Error Responses

**Condition** : If email Not found.

**Code** : `404 NOT FOUND`

**Content example** : 

```json
{
    "code": 404,
    "message": "Not found"
}
```

### Or

**Condition** : If fields are missed.

**Code** : `400 BAD REQUEST`

**Content example**

```json
{
    "code": 400,
    "message": "Please specify your email or password"
}
```