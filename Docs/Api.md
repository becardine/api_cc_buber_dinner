# Buber Dinner API

+ [Buber Dinner API](#buber-dinner-api)
  + [Auth](#auth)
    + [Register](#register)
      + [Register Request](#register-request)
      + [Register Response](#register-response)
    + [Login](#login)
      + [Login Request](#login-request)
      + [Login Response](#login-response)

## Auth

### Register

```js
POST {{host}}/auth/register
```

#### Register Request

```json
{
	"firstName": "John",
	"lastName": "Doe",
	"email": "john@doe.com",
	"password": "JohnDoe"
}
```

#### Register Response

```js
200 OK
```

```json
{
	"id": "b032727f-0b5e-46c2-b3b9-5b3f0159ae74",
	"firstName": "John",
	"lastName": "Doe",
	"email": "john@doe.com",
	"token": "eyJGb...z9aSdwYoI"
}
```

### Login

```js
POST {{host}}/auth/login
```

#### Login Request

```json
{
	"email": "john@doe.com",
	"password": "JohnDoe"
}
```

#### Login Response

```js
200 OK
```

```json
{
	"id": "b032727f-0b5e-46c2-b3b9-5b3f0159ae74",
	"firstName": "John",
	"lastName": "Doe",
	"email": "john@doe.com",
	"token": "eyJGb...z9aSdwYoI"
}
```
