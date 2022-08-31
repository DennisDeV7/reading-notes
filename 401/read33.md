# Authentication and Production Server

## JSON Web Tokens

A JSON web token is a way to send information securely using a JSON object. They are typically used when authorization is needed or information is exchanged.

The JSON Web Token is structured with three parts: header, payload, and signature (xxxxx.yyyyy.zzzzz)

The header has two parts: type of token, and the signing algorithm

```txt
{
  "alg": "HS256",
  "typ": "JWT"
}
```

The payload contains the claims which looks like:

```txt
{
  "sub": "1234567890",
  "name": "John Doe",
  "admin": true
}
```

The signature does as it sounds and signs the encoded parts of the token in order to verify the message and looks like this:

```txt
HMACSHA256(
  base64UrlEncode(header) + "." +
  base64UrlEncode(payload),
  secret)s
```

can be installed with `pip install djangorestframework_simplejwt`

In a django rest framework the views, urls, and settings must be updated as well. See [this tutorial](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html) for specific instructions.

## Things I want to learn more about