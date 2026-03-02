# User API Specification

## Create User

Endpoint : POST `/api/users`

Request Body :

```json
{
  "name" : "lala",
  "age" : 16
}
```

Response Body (success) :

```json
{
  "status": "success",
  "data": {
    "id" : "886864ea-6eb7-4540-867c-561997a1a30c",
    "name": "lala",
    "age": 16
  }
}
```

Response Body (failed) :

```json
{
  "error": "Invalid input data"
}
```

## Update User

Endpoint : PUT `/api/users/{id}`

Request Body :

```json
{
  "name" : "lala Updated",
  "age" : 18
}
```

Response Body (success) :

```json
{
  "status": "success",
  "data": {
    "id" : "886864ea-6eb7-4540-867c-561997a1a30c",
    "name": "lala Updated",
    "age": 18
  }
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```

## Get User

Endpoint : GET `/api/users`

Response Body (success) :

```json
{
  "status": "success",
  "data": [
    {
      "id" : "886864ea-6eb7-4540-867c-561997a1a30c",
      "name": "lala",
      "age": 16
    }
  ]
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```

## Delete User

Endpoint : DELETE `/api/users/{id}`

Response Body (success) :

```json
{
  "status": "success delete user with id 886864ea-6eb7-4540-867c-561997a1a30c"
}
```

Response Body (failed) :

```json
{
  "error": "User not found"
}
```


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/acc03a03-1a00-46d6-a369-285f24d95a94" />
