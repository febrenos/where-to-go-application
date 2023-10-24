# Where2Go

#### 1. Introdução
Java Spring Boot como framework de backend e baseada na arquitetura RESTful.
- http://localhost:8080


| Method | url |
|---|---|
| POST | /trip |
| POST | /login |
| POST | /user/register |
| GET | /users |
| GET | /message |
| DEL | /message |

<details>
<summary>/trip</summary>
    
- request
```json
{
  "clima": "quente",
  "transporte": "avião",
  "tempoMaximo": 7,
  "custoMaximo": 10000.00
}
```

</details>
<details>
<summary>/login</summary>

- requests
```json
{
  "login": "neurotrix@fiap.com",
  "password": "teste123"
}
```

</details>

<details>
<summary>/register</summary>

- requests
```json
{
  "name": "Leandro",
  "email": "neurotrix@fiap.com",
  "password": "teste123"
}
```

</details>

<details>
<summary>/users</summary>

- response
```json
{
    "_embedded": {
        "users": [
            {
                "name": "Leandro",
                "email": "neurotrix@fiap.com",
                "password": "$2a$10$1auG/AZlcd6LzB/yhgboyuKbn0biU.eEw3wUa9gA5d4KV3eLhY/5u",
                "dateOfBirth": null,
                "role": "USER",
                "preferences": [],
                "enabled": true,
                "authorities": [
                    {
                        "authority": "USER"
                    }
                ],
                "username": "neurotrix@fiap.com",
                "accountNonLocked": true,
                "accountNonExpired": true,
                "credentialsNonExpired": true,
                "_links": {
                    "self": {
                        "href": "http://localhost:8080/users/1"
                    },
                    "user": {
                        "href": "http://localhost:8080/users/1"
                    },
                    "trips": {
                        "href": "http://localhost:8080/users/1/trips"
                    },
                    "address": {
                        "href": "http://localhost:8080/users/1/address"
                    },
                    "messages": {
                        "href": "http://localhost:8080/users/1/messages"
                    },
                    "bookings": {
                        "href": "http://localhost:8080/users/1/bookings"
                    }
                }
            }
        ]
    },
    "_links": {
        "self": {
            "href": "http://localhost:8080/users"
        },
        "profile": {
            "href": "http://localhost:8080/profile/users"
        },
        "search": {
            "href": "http://localhost:8080/users/search"
        }
    },
    "page": {
        "size": 20,
        "totalElements": 1,
        "totalPages": 1,
        "number": 0
    }
}
```

</details>

<details>
<summary>/message</summary>

- requests
```json
```

</details>

<details>
<summary>/message/{id}</summary>

- requests
```json
```

</details>





