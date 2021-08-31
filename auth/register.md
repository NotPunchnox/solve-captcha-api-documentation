# Create User's Account


**URL** : `https://solve-captcha.herokuapp.com/auth/register/`

**Method** : `POST`

**Data constraints**

```json
{
    "email": "email",
    "password": "[unicode 5 chars min]"
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

**Code** : `201 CREATED`

**Content example**

```json
{
    "code": 201,
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJJRCI6NDUwMDE2MzA0MTY1NDM3MDAsImlhdCI6MTYzMDQxNjU0M30.JhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9-jazgz5-aA"
}
```

## Error Responses

**Condition** : If email already used for User.

**Code** : `403 FORBIDDEN`

**Content example** : 

```json
{
    "code": 403,
    "message": "The email already used"
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