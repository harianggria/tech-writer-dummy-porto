# API Testing – Create User (POST /api/users)

## Purpose
To verify that a new user can be successfully created using the Reqres API.

## Endpoint
`POST https://reqres.in/api/users`

## Request Headers
| Key           | Value                    |
|---------------|--------------------------|
| x-api-key     | reqres-free-v1           |
| Content-Type  | application/json         |

## Request Body
```json
{
  "first_name": "Ria",
  "last_name": "Anggriani",
  "avatar": "https://avatars.githubusercontent.com/u/9919?s=200&v=4"
}
```

## Expected Result 
The expected result should be :
- Status Code: 201 Created
- Body 
```
{
    "first_name": "Ria",
    "last_name": "Anggriani",
    "avatar": "https://avatars.githubusercontent.com/u/9919?s=200&v=4",
    "id": "generated_id",
    "createdAt": "timestamp"
}
```
