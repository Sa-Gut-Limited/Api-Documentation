# Project: My Sass
# 📁 Collection: Admin 


>```
> {{Production Base Url}} =>  "https://backend-dev-si6tfq.laravel.cloud"
> {{Dev Base Url}}       =>  "https://backend-main-al4zzr.laravel.cloud"
>```


## End-point: Login
### Method: POST
>```
>{{baseurl}}/api/v1/auth/admin/login
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Payload (**raw**)

```json
{
   "email" : "owurakwaku758@gmail.com",
   "password" : "owurakwaku@2"
}
```

### Response: 200
```json
{
    "message": "Login successful",
    "token": "6|8krJRhvGaS4j0xQ9Udf2qW1YHUVwhbaRfsAi3Eo1e9f8a8b9"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: SignUp
### Method: POST
>```
>{{baseurl}}/api/v1/auth/admin/signup
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Body (**raw**)

```json
{
    "name"  :  "Owura Safo",                  // Required
    "email"      : "owurakwaku758@gmail.com", // Required
    "password"   : "owurakwaku@2",            // Required
    "password_confirmation" : "owurakwaku@2", // Required
    "phone"   : "+233500081395",              // Required
    "image" : {{image}}                       // Nullable
}
```

### Response: 201
```json
{
    "message": "User created successfully",
    "user": {
        "name": "Owura Safo",
        "email": "owurakwaku165@gmail.com",
        "phone": "+233500081395",
        "image": null,
        "updated_at": "2025-05-07T17:20:33.000000Z",
        "created_at": "2025-05-07T17:20:33.000000Z",
        "id": 1
    },
    "token": "5|ExhB1xBBhs87wUoZTVqDNzY04sSmebZZ0N6YTNCh77849027"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Logout
### Method: DELETE
>```
>{{baseurl}}/api/v1/auth/admin/logout
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Logout successful"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Refreshtoken
### Method: GET
>```
>{{baseurl}}/api/v1/auth/users/refresh
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{admintoken}}|string|


### Response: 200
```json
{
    "message": "Token refreshed successfully",
    "token": "8|sNoC0EhSjsp52JlejHDVnkrJ3L51p7VG1vE2muXY516de16c"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Reset-Password
### Method: PATCH
>```
>{{baseurl}}/api/v1/auth/admin/reset-password
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Body (**raw**)

```json
{
   "old_password" : "owurakwaku@1",
   "new_password" : "Owurasafo@2",
   "password_confirmation" : "Owurasafo@2"
   
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|



