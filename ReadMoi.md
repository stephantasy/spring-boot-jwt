The code comes from : 

```sh
https://www.javainuse.com/spring/boot-jwt
```

To test the project, use POSTMAN:

## Fetch the TOKEN

- Create a `POST` request using the path:
```
http://localhost:8083/authenticate
```
- Choose the `Body` tab
- Put the text below as a `raw` and `JSON(application/json` data:
```
{
"username":"javainuse",
"password":"password"
}
```

Copy the TOKEN that you get:
```
{
    "token": "eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJqYXZhaW51c2UiLCJleHAiOjE1NjM4OTU1NTMsImlhdCI6MTU2Mzg3NzU1M30.ROUKHriNohZieSXvHCXvG9p0WMtdPj-Cid4qLJoVm3k"
}
```

## Get the data

- Create a `GET` request using the path:
```
http://localhost:8083/hello
```
- Choose the `Authorization` tab
- Choose the `OAuth 2.0` type
- Copy your Token in the `Acess Token` field