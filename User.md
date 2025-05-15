# 📁 Collection: User 


>```
> {{Production Base Url}} =>  "https://backend-dev-si6tfq.laravel.cloud"
> {{Dev Base Url}}       =>  "https://backend-main-al4zzr.laravel.cloud"
>```

## End-point: Login
### Method: POST
>```
>{{baseurl}}/api/v1/auth/users/login
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
   "email" : "de.azaglo@gmail.com",
   "password" : "azaglo1"
}
```

### Response: 200
```json
{
    "message": "User Logged in successful",
    "token": "2|kLrKZjHz7AtwYzdopcsn02reu0naj8gv4HBIqMZxcf93ec01"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: SignUp
### Method: POST
>```
>{{baseurl}}/api/v1/auth/users/signup
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
    "first_name" : "Derrick ",
    "last_name"  : "Azaglo",
    "email"      : "de.azaglo@gmail.com",
    "password"   : "azaglo1",
    "phone"      : "+233549632604",
    "password_confirmation" : "azaglo1",
    "date_of_birth" : "11/06/2003",
    //image is nullable
    "image" :{{image1}}
}
```

### Response: 201
```json
{
    "message": "User created successfully",
    "user": {
        "first_name": "Owura",
        "last_name": "kwaku Safo",
        "email": "owurakwaku758@gmail.com",
        "Date_of_Birth": "11/06/2003",
        "image": null,
        "updated_at": "2025-05-07T17:15:34.000000Z",
        "created_at": "2025-05-07T17:15:34.000000Z",
        "id": 1
    },
    "token": "1|tHlqsxNompJPzWGZ4fE9ztwWEtrU2ZH0TV5JJzaB1ef6295e"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Logout
### Method: POST
>```
>{{baseurl}}/api/v1/auth/users/logout
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
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Token refreshed successfully",
    "token": "4|b3teWAtjfJ3vPHNeCgGcJNMicHScGjlnqqOx3AYGbab315ea"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Reset-Password
### Method: POST
>```
>{{baseurl}}/api/v1/auth/users/reset-password
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
    "email" : "de.azaglo@gmail.com"
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Password reset link sent to your email"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Profile
### Method: GET
>```
>{{baseurl}}/api/v1/users/profile
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Query Params

|Param|value|
|---|---|
||null|


### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "User Details",
    "data": {
        "id": 1,
        "first_name": "Owura",
        "last_name": "kwaku Safo",
        "email": "owurakwaku758@gmail.com",
        "phone": "+233500081395",
        "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746913218/image/ps3xkkpjxourx5ajtwze.jpg"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Update Profile
### Method: PATCH
>```
>{{baseurl}}/api/v1/users/profile/{user_id}
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
    "first_name" : "",       //Sometimes 
    "last_name"  : "",       // Sometimes
    "email"      : "",       // Sometimes
    "date_of_birth" : "",    // Sometimes
    "phone"      : "+233500081395"  // Sometimes
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "User Updated Successfully",
    "data": {
        "id": 1,
        "first_name": "Owura",
        "last_name": "kwaku Safo",
        "email": "owurakwaku758@gmail.com",
        "phone": "+233500081395",
        "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746913218/image/ps3xkkpjxourx5ajtwze.jpg"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Delete User
### Method: DELETE
>```
>{{baseurl}}/api/v1/users/profile/1
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



⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get Categories
### Method: GET
>```
>{{baseurl}}/api/v1/users/category
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
    "message": "Categories retrieved successfully",
    "data": {
        "list": [
            {
                "id": 1,
                "name": "Chair",
                "created_at": "2025-05-10T21:40:46.000000Z"
            }
        ],
        "pagination": {
            "count": 1,
            "total": 1,
            "current_page": 1,
            "last_page": 1,
            "per_page": 15
        }
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get Category
### Method: GET
>```
>{{baseurl}}/api/v1/users/category/{category_id}
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
    "message": "Category Retrieved Successfully",
    "data": {
        "id": 1,
        "name": "Chair",
        "created_at": "2025-05-10T21:40:46.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Create Category
### Method: POST
>```
>{{baseurl}}/api/v1/users/category
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
    "name" : "Shoe"
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Category Created Successfully",
    "data": {
        "id": 1,
        "name": "Shoe",
        "created_at": "2025-05-10T21:40:46.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Update Category
### Method: PATCH
>```
>{{baseurl}}/api/v1/users/category/{category_id}
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
    "name" : "Table"
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Category Updated Successfully",
    "data": {
        "id": 2,
        "name": "Table",
        "created_at": "2025-05-11T13:48:08.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Delete Category
### Method: DELETE
>```
>{{baseurl}}/api/v1/users/category/{category_id}
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
    "message": "Category Deleted Successfully"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get all Products
### Method: GET
>```
>{{baseurl}}/api/v1/users/product
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Query Params

|Param|value|
|---|---|
|search|bed|


### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Products retrieved successfully",
    "data": {
        "list": [
            {
                "id": 4,
                "name": "baggy jeans",
                "description": "This is a sample product description.",
                "size": "Medium",
                "category": {
                    "id": 1,
                    "name": "Chair"
                },
                "tag": null,
                "price": "99.99",
                "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746972091/image/xhq4hn8ur71ielgurvui.jpg",
                "currency": "GHS",
                "width": "10.50",
                "height": "15.00",
                "weight": null,
                "sku": "BBe040",
                "cost_price": null,
                "selling_price": "120.00",
                "slug": "baggy-jeans-3a7d244c-82bf-4422-ae7a-16fc1317771b",
                "is_out_of_stock": 0,
                "is_disabled": 0,
                "rating_count": 0,
                "rating": "0.00",
                "is_favorite": false,
                "created_at": "2025-05-11T14:01:32.000000Z"
            },
            {
                "id": 3,
                "name": "Shoe",
                "description": "This is a sample product description.",
                "size": "Medium",
                "category": {
                    "id": 1,
                    "name": "Chair"
                },
                "tag": null,
                "price": "99.99",
                "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746971623/image/zin52g7xxlfchdeccvxz.jpg",
                "currency": "GHS",
                "width": "10.50",
                "height": "15.00",
                "weight": null,
                "sku": "Shoe040",
                "cost_price": null,
                "selling_price": "120.00",
                "slug": "shoe-8ec12bc1-e5e2-4d39-ac45-55f34c0b80e9",
                "is_out_of_stock": 0,
                "is_disabled": 0,
                "rating_count": 0,
                "rating": "0.00",
                "is_favorite": false,
                "created_at": "2025-05-11T13:53:44.000000Z"
            },
            {
                "id": 2,
                "name": "Hand Bag",
                "description": "This is a sample product description.",
                "size": "Medium",
                "category": {
                    "id": 1,
                    "name": "Chair"
                },
                "tag": null,
                "price": "99.99",
                "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746971424/image/daysrdp5spgzwvjkzyg7.jpg",
                "currency": "GHS",
                "width": "10.50",
                "height": "15.00",
                "weight": null,
                "sku": "HB2365",
                "cost_price": null,
                "selling_price": "120.00",
                "slug": "hand-bag-e58a9395-788d-469f-bdb0-91a7399d5e50",
                "is_out_of_stock": 0,
                "is_disabled": 0,
                "rating_count": 0,
                "rating": "0.00",
                "is_favorite": false,
                "created_at": "2025-05-11T13:50:24.000000Z"
            }
        ],
        "pagination": {
            "count": 3,
            "total": 3,
            "current_page": 1,
            "last_page": 1,
            "per_page": 15
        }
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get Product Details
### Method: GET
>```
>{{baseurl}}/api/v1/users/product/{product_id}
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Response: 200
```json
{
    "message": "Product retrieved successfully",
    "data": {
        "id": 4,
        "name": "baggy jeans",
        "description": "This is a sample product description.",
        "size": "Medium",
        "category": {
            "id": 1,
            "name": "Chair"
        },
        "tag": null,
        "price": "99.99",
        "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746972091/image/xhq4hn8ur71ielgurvui.jpg",
        "currency": "GHS",
        "width": "10.50",
        "height": "15.00",
        "weight": null,
        "sku": "BBe040",
        "cost_price": null,
        "selling_price": "120.00",
        "slug": "baggy-jeans-3a7d244c-82bf-4422-ae7a-16fc1317771b",
        "is_out_of_stock": 0,
        "is_disabled": 0,
        "rating_count": 0,
        "rating": "0.00",
        "is_favorite": false,
        "created_at": "2025-05-11T14:01:32.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Create a Prodcut
### Method: POST
>```
>{{baseurl}}/api/v1/users/product
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
  "name": "Test Product",
  "description": "This is a sample product description.",
  "size": "Medium",
  "category_id": 1,
  "price": 99.99,
  "currency": "GHS",
  "width": 10.5,
  "height": 15.0,
  "weight": 1.2,
  "sku": "HOGAe040",
  "images": [
    {
      "image":{{image2}},
      "is_primary": true,   // Is primary is the main image and display order will be how the image will be arranged
      "display_order": 1
    },
    {
      "image":{{image3}},
      "display_order": 2
    }
  ]
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 201
```json
{
    "message": "Product created successfully",
    "data": {
        "id": null,
        "name": null,
        "description": null,
        "size": null,
        "category": null,
        "tag": null,
        "price": null,
        "image": null,
        "currency": null,
        "width": null,
        "height": null,
        "weight": null,
        "sku": null,
        "cost_price": null,
        "selling_price": null,
        "slug": null,
        "is_out_of_stock": null,
        "is_disabled": null,
        "rating_count": null,
        "rating": null,
        "is_favorite": false,
        "created_at": null
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Update a Product
### Method: PATCH
>```
>{{baseurl}}/api/v1/users/product/{product_id}
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
    "price" : 2.00
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Product updated successfully",
    "data": {
        "id": 2,
        "name": "Hand Bag",
        "description": "This is a sample product description.",
        "size": "Medium",
        "category": {
            "id": 1,
            "name": "Chair"
        },
        "tag": null,
        "price": 2,
        "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746971424/image/daysrdp5spgzwvjkzyg7.jpg",
        "currency": "GHS",
        "width": "10.50",
        "height": "15.00",
        "weight": null,
        "sku": "HB2365",
        "cost_price": null,
        "selling_price": "120.00",
        "slug": "hand-bag-e58a9395-788d-469f-bdb0-91a7399d5e50",
        "is_out_of_stock": 0,
        "is_disabled": 0,
        "rating_count": 0,
        "rating": "0.00",
        "is_favorite": false,
        "created_at": "2025-05-11T13:50:24.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Product Filter
### Method: GET
>```
>{{baseurl}}/api/v1/users/product/filters?is_out_of_stock=0
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Query Params

|Param|value|
|---|---|
|category_id|0|
|min_price|null|   // Filter based on the min_price and max_price  |int|
|is_out_of_stock|0|   // boolean |true|false|


### Response: 200
```json
{
    "message": "Product retrieved successfully",
    "data": {
        "list": [
            {
                "id": 2,
                "name": "Hand Bag",
                "description": "This is a sample product description.",
                "size": "Medium",
                "category": {
                    "id": 1,
                    "name": "Chair"
                },
                "tag": null,
                "price": "2.00",
                "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746971424/image/daysrdp5spgzwvjkzyg7.jpg",
                "currency": "GHS",
                "width": "10.50",
                "height": "15.00",
                "weight": null,
                "sku": "HB2365",
                "cost_price": null,
                "selling_price": "120.00",
                "slug": "hand-bag-e58a9395-788d-469f-bdb0-91a7399d5e50",
                "is_out_of_stock": 0,
                "is_disabled": 0,
                "rating_count": 0,
                "rating": "0.00",
                "is_favorite": false,
                "created_at": "2025-05-11T13:50:24.000000Z"
            },
            {
                "id": 3,
                "name": "Shoe",
                "description": "This is a sample product description.",
                "size": "Medium",
                "category": {
                    "id": 1,
                    "name": "Chair"
                },
                "tag": null,
                "price": "99.99",
                "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746971623/image/zin52g7xxlfchdeccvxz.jpg",
                "currency": "GHS",
                "width": "10.50",
                "height": "15.00",
                "weight": null,
                "sku": "Shoe040",
                "cost_price": null,
                "selling_price": "120.00",
                "slug": "shoe-8ec12bc1-e5e2-4d39-ac45-55f34c0b80e9",
                "is_out_of_stock": 0,
                "is_disabled": 0,
                "rating_count": 0,
                "rating": "0.00",
                "is_favorite": false,
                "created_at": "2025-05-11T13:53:44.000000Z"
            },
            {
                "id": 4,
                "name": "baggy jeans",
                "description": "This is a sample product description.",
                "size": "Medium",
                "category": {
                    "id": 1,
                    "name": "Chair"
                },
                "tag": null,
                "price": "99.99",
                "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746972091/image/xhq4hn8ur71ielgurvui.jpg",
                "currency": "GHS",
                "width": "10.50",
                "height": "15.00",
                "weight": null,
                "sku": "BBe040",
                "cost_price": null,
                "selling_price": "120.00",
                "slug": "baggy-jeans-3a7d244c-82bf-4422-ae7a-16fc1317771b",
                "is_out_of_stock": 0,
                "is_disabled": 0,
                "rating_count": 0,
                "rating": "0.00",
                "is_favorite": false,
                "created_at": "2025-05-11T14:01:32.000000Z"
            }
        ],
        "pagination": {
            "count": 3,
            "total": 3,
            "current_page": 1,
            "last_page": 1,
            "per_page": 15
        }
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Product Search
### Method: GET
>```
>{{baseurl}}/api/v1/users/product/search?s=te
>```
### Headers

|Content-Type|Value|
|---|---|
|Accept|application/json|


### Headers

|Content-Type|Value|
|---|---|
|Content-Type|application/json|


### Query Params

|Param|value|
|search| product_name|
|---  |---|
|s|te|       // Use s for the search parameter


### Response: 200
```json
{
    "message": "Product retrieved successfully",
    "data": {
        "list": [
            {
                "id": 2,
                "name": "Hand Bag",
                "description": "This is a sample product description.",
                "size": "Medium",
                "price": "2.00",
                "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746971424/image/daysrdp5spgzwvjkzyg7.jpg",
                "currency": "GHS",
                "width": "10.50",
                "height": "15.00",
                "weight": null,
                "sku": "HB2365",
                "cost_price": null,
                "selling_price": "120.00",
                "slug": "hand-bag-e58a9395-788d-469f-bdb0-91a7399d5e50",
                "is_out_of_stock": 0,
                "is_disabled": 0,
                "rating_count": 0,
                "rating": "0.00",
                "is_favorite": false,
                "created_at": "2025-05-11T13:50:24.000000Z"
            }
        ],
        "pagination": {
            "count": 1,
            "total": 1,
            "current_page": 1,
            "last_page": 1,
            "per_page": 15
        }
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Delete a Product
### Method: DELETE
>```
>{{baseurl}}/api/v1/users/product/{product_id}
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
    "message": "Product deleted successfully"
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Add to Favorite
### Method: POST
>```
>{{baseurl}}/api/v1/users/product/favorite
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
    "product_id" : 1
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Product favorite added successfully",
    "data": {
        "id": 2,
        "name": "Hand Bag",
        "description": "This is a sample product description.",
        "size": "Medium",
        "price": "2.00",
        "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746971424/image/daysrdp5spgzwvjkzyg7.jpg",
        "currency": "GHS",
        "width": "10.50",
        "height": "15.00",
        "weight": null,
        "sku": "HB2365",
        "cost_price": null,
        "selling_price": "120.00",
        "slug": "hand-bag-e58a9395-788d-469f-bdb0-91a7399d5e50",
        "is_out_of_stock": 0,
        "is_disabled": 0,
        "rating_count": 0,
        "rating": "0.00",
        "is_favorite": true,
        "created_at": "2025-05-11T13:50:24.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Remove from Favorite
### Method: DELETE
>```
>{{baseurl}}/api/v1/users/product/favorite/{product_id}
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

```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Product favorite removed successfully",
    "data": {
        "id": 3,
        "name": "baggy jeans",
        "description": "This is a sample product description.",
        "size": "Medium",
        "price": "99.99",
        "image": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746974622/image/btvctvsejiacys94x62h.jpg",
        "currency": "GHS",
        "width": "10.50",
        "height": "15.00",
        "weight": null,
        "sku": "BAe040",
        "cost_price": null,
        "selling_price": "120.00",
        "slug": "baggy-jeans",
        "is_out_of_stock": 0,
        "is_disabled": 0,
        "rating_count": 0,
        "rating": "0.00",
        "is_favorite": false,
        "created_at": "2025-05-11T14:43:43.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get All ratings
### Method: GET
>```
>{{baseurl}}/api/v1/users/rating
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
    "message": "Product reviews retrieved successfully",
    "data": [
        {
            "id": 1,
            "user": {
                "id": 1,
                "name": "Owura kwaku Safo"
            },
            "product": {
                "id": 2,
                "name": "baggy jeans"
            },
            "rating": 5,
            "comments": "This product is great"
        },
        {
            "id": 2,
            "user": {
                "id": 1,
                "name": "Owura kwaku Safo"
            },
            "product": {
                "id": 2,
                "name": "baggy jeans"
            },
            "rating": 5,
            "comments": "This product is great"
        },
        {
            "id": 3,
            "user": {
                "id": 1,
                "name": "Owura kwaku Safo"
            },
            "product": {
                "id": 2,
                "name": "baggy jeans"
            },
            "rating": 5,
            "comments": "This product is great"
        }
    ]
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get Product Details
### Method: GET
>```
>{{baseurl}}/api/v1/users/rating/{rating_id}
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
    "message": "Product review fetched successfully",
    "data": {
        "id": 1,
        "user": {
            "id": 1,
            "name": "Owura kwaku Safo"
        },
        "product": {
            "id": 2,
            "name": "baggy jeans"
        },
        "rating": 5,
        "comments": "This product is great"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get Products Ratings
### Method: GET
>```
>{{baseurl}}/api/v1/users/rating/{product_id}/product
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
// api/v1/users/rating/{product_id}/product
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Product reviews retrieved successfully",
    "data": {
        "list": [
            {
                "id": 1,
                "user": {
                    "id": 1,
                    "name": "Owura kwaku Safo"
                },
                "rating": 5,
                "comments": "This product is great"
            },
            {
                "id": 2,
                "user": {
                    "id": 1,
                    "name": "Owura kwaku Safo"
                },
                "rating": 5,
                "comments": "This product is great"
            },
            {
                "id": 3,
                "user": {
                    "id": 1,
                    "name": "Owura kwaku Safo"
                },
                "rating": 5,
                "comments": "This product is great"
            }
        ],
        "pagination": {
            "count": 3,
            "total": 3,
            "current_page": 1,
            "last_page": 1,
            "per_page": 15
        }
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Create a Rating
### Method: POST
>```
>{{baseurl}}/api/v1/users/rating
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
    "user_id" : "1",
    "product_id" : "1",
    "rating"  : "5",
    "comments"  : "I love this product"    // nullable
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 201
```json
{
    "message": "Product review created successfully",
    "data": {
        "id": 4,
        "rating": "4",
        "comments": "This product is great"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get Orders
### Method: GET
>```
>{{baseurl}}/api/v1/users/order/
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
    "message": "Orders retrieved successfully",
    "data": {
        "list": [
            {
                "id": 12,
                "order_number": "20250514YPYRA2",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 12,
                    "created_at": "2025-05-14T18:07:00.000000Z"
                },
                "items": [
                    {
                        "id": 1,
                        "quantity": 7,
                        "price": null,
                        "total": "0.00",
                        "product": {
                            "id": 1,
                            "name": "Test Product",
                            "description": "This is a sample product description.",
                            "price": "99.99",
                            "image": null,
                            "sku": "HOLAe040"
                        }
                    },
                    {
                        "id": 2,
                        "quantity": 2,
                        "price": null,
                        "total": "0.00",
                        "product": {
                            "id": 2,
                            "name": "Test Product",
                            "description": "This is a sample product description.",
                            "price": "99.99",
                            "image": null,
                            "sku": "HOGAe040"
                        }
                    }
                ]
            },
            {
                "id": 11,
                "order_number": "20250514K3MY4P",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 11,
                    "created_at": "2025-05-14T18:06:27.000000Z"
                },
                "items": []
            },
            {
                "id": 10,
                "order_number": "20250514KYSG5N",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 10,
                    "created_at": "2025-05-14T17:59:41.000000Z"
                },
                "items": []
            },
            {
                "id": 9,
                "order_number": "20250514QVAIU0",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 9,
                    "created_at": "2025-05-14T17:56:26.000000Z"
                },
                "items": []
            },
            {
                "id": 8,
                "order_number": "20250514W2PJS2",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 8,
                    "created_at": "2025-05-14T17:54:19.000000Z"
                },
                "items": []
            },
            {
                "id": 7,
                "order_number": "20250514BX50KM",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 7,
                    "created_at": "2025-05-14T17:52:26.000000Z"
                },
                "items": []
            },
            {
                "id": 6,
                "order_number": "20250514E77M3N",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 6,
                    "created_at": "2025-05-14T17:51:49.000000Z"
                },
                "items": []
            },
            {
                "id": 5,
                "order_number": "20250514QD5HMF",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 5,
                    "created_at": "2025-05-14T17:50:46.000000Z"
                },
                "items": []
            },
            {
                "id": 4,
                "order_number": "20250514Z8VWVO",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 4,
                    "created_at": "2025-05-14T17:50:06.000000Z"
                },
                "items": []
            },
            {
                "id": 3,
                "order_number": "202505149EGSOP",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 3,
                    "created_at": "2025-05-14T17:49:55.000000Z"
                },
                "items": []
            },
            {
                "id": 2,
                "order_number": "20250514O5PIXX",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 2,
                    "created_at": "2025-05-14T17:47:02.000000Z"
                },
                "items": []
            },
            {
                "id": 1,
                "order_number": "20250514SZXP9D",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 1,
                    "created_at": "2025-05-14T17:45:47.000000Z"
                },
                "items": []
            }
        ],
        "pagination": {
            "count": 12,
            "total": 12,
            "current_page": 1,
            "last_page": 1,
            "per_page": 15
        }
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Order History
### Method: GET
>```
>{{baseurl}}/api/v1/users/order/history
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
    "message": "Order history retrieved successfully",
    "data": {
        "list": [
            {
                "id": 12,
                "order_number": "20250514YPYRA2",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 12,
                    "created_at": "2025-05-14T18:07:00.000000Z"
                },
                "items": [
                    {
                        "id": 1,
                        "quantity": 7,
                        "price": null,
                        "total": "0.00",
                        "product": {
                            "id": 1,
                            "name": "Test Product",
                            "description": "This is a sample product description.",
                            "price": "99.99",
                            "image": null,
                            "sku": "HOLAe040"
                        }
                    },
                    {
                        "id": 2,
                        "quantity": 2,
                        "price": null,
                        "total": "0.00",
                        "product": {
                            "id": 2,
                            "name": "Test Product",
                            "description": "This is a sample product description.",
                            "price": "99.99",
                            "image": null,
                            "sku": "HOGAe040"
                        }
                    }
                ]
            },
            {
                "id": 11,
                "order_number": "20250514K3MY4P",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 11,
                    "created_at": "2025-05-14T18:06:27.000000Z"
                },
                "items": []
            },
            {
                "id": 10,
                "order_number": "20250514KYSG5N",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 10,
                    "created_at": "2025-05-14T17:59:41.000000Z"
                },
                "items": []
            },
            {
                "id": 9,
                "order_number": "20250514QVAIU0",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 9,
                    "created_at": "2025-05-14T17:56:26.000000Z"
                },
                "items": []
            },
            {
                "id": 8,
                "order_number": "20250514W2PJS2",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 8,
                    "created_at": "2025-05-14T17:54:19.000000Z"
                },
                "items": []
            },
            {
                "id": 7,
                "order_number": "20250514BX50KM",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 7,
                    "created_at": "2025-05-14T17:52:26.000000Z"
                },
                "items": []
            },
            {
                "id": 6,
                "order_number": "20250514E77M3N",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 6,
                    "created_at": "2025-05-14T17:51:49.000000Z"
                },
                "items": []
            },
            {
                "id": 5,
                "order_number": "20250514QD5HMF",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 5,
                    "created_at": "2025-05-14T17:50:46.000000Z"
                },
                "items": []
            },
            {
                "id": 4,
                "order_number": "20250514Z8VWVO",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 4,
                    "created_at": "2025-05-14T17:50:06.000000Z"
                },
                "items": []
            },
            {
                "id": 3,
                "order_number": "202505149EGSOP",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 3,
                    "created_at": "2025-05-14T17:49:55.000000Z"
                },
                "items": []
            },
            {
                "id": 2,
                "order_number": "20250514O5PIXX",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 2,
                    "created_at": "2025-05-14T17:47:02.000000Z"
                },
                "items": []
            },
            {
                "id": 1,
                "order_number": "20250514SZXP9D",
                "status": "pending",
                "subtotal": "0.00",
                "tax": "0.00",
                "shipping_cost": "0.00",
                "discount": "0.00",
                "total_amount": "0.00",
                "notes": null,
                "lat": "5.667783",
                "lng": "-0.166718",
                "user": {
                    "id": 1,
                    "name": null,
                    "email": "de.azaglo@gmail.com",
                    "phone": "+233549632604"
                },
                "order_group": {
                    "id": 1,
                    "created_at": "2025-05-14T17:45:47.000000Z"
                },
                "items": []
            }
        ],
        "pagination": {
            "count": 12,
            "total": 12,
            "current_page": 1,
            "last_page": 1,
            "per_page": 15
        }
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get User Order
### Method: GET
>```
>{{baseurl}}/api/v1/users/order/{order_id}
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
    "message": "Order retrieved successfully",
    "data": {
        "id": 12,
        "order_number": "20250514YPYRA2",
        "status": "pending",
        "subtotal": "0.00",
        "tax": "0.00",
        "shipping_cost": "0.00",
        "discount": "0.00",
        "total_amount": "0.00",
        "notes": null,
        "lat": "5.667783",
        "lng": "-0.166718",
        "user": {
            "id": 1,
            "name": null,
            "email": "de.azaglo@gmail.com",
            "phone": "+233549632604"
        },
        "order_group": {
            "id": 12,
            "created_at": "2025-05-14T18:07:00.000000Z"
        },
        "items": [
            {
                "id": 1,
                "quantity": 7,
                "price": null,
                "total": "0.00",
                "product": {
                    "id": 1,
                    "name": "Test Product",
                    "description": "This is a sample product description.",
                    "price": "99.99",
                    "image": null,
                    "sku": "HOLAe040"
                }
            },
            {
                "id": 2,
                "quantity": 2,
                "price": null,
                "total": "0.00",
                "product": {
                    "id": 2,
                    "name": "Test Product",
                    "description": "This is a sample product description.",
                    "price": "99.99",
                    "image": null,
                    "sku": "HOGAe040"
                }
            }
        ]
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Pay For Orders
### Method: POST
>```
>{{baseurl}}/api/v1/users/order/{order_id}/pay
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
    "payment_method" : "paystack",   // cash or Paystack 
    "account_number" : "+233500081395",
    "provider"        : "telecel"   // Null when payment_method is cash
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Payment initiated",
    "data": {
        "checkoutUrl": "https://checkout.paystack.com/kn9w29lsr3wxyw1",
        "accessCode": "kn9w29lsr3wxyw1",
        "reference": "6hiclez166",
        "orderId": 1
    }
}
```
### Response 200

```json
{
    "message": "Pay cash on order delivery",
    "data": {
        "checkoutUrl": null,
        "accessCode": null,
        "reference": null
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Cancel an Order
### Method: PATCH
>```
>{{baseurl}}/api/v1/users/order/{order_id}/cancel
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
    "message": "Order canceled successfully",
    "data": {
        "id": 3,
        "order_number": "20250515KKDU8O",
        "status": "cancelled",
        "subtotal": "99.99",
        "tax": "0.00",
        "shipping_cost": "0.00",
        "discount": "0.00",
        "total_amount": "99.99",
        "amount_paid": "0.00",
        "payment_method": null,
        "payment_status": "unpaid",
        "amount_due": 99.99,
        "notes": null,
        "lat": "5.667783",
        "lng": "-0.166718",
        "address": "MR9M+376, Madina",
        "created_at": "2025-05-15T16:50:11.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Re0rder
### Method: POST
>```
>{{baseurl}}/api/v1/users/order/{order_id}/reOrder
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
    "message": "Order re-created successfully",
    "data": {
        "id": 3,
        "order_number": "20250515KKDU8O",
        "status": "pending",
        "subtotal": "99.99",
        "tax": "0.00",
        "shipping_cost": "0.00",
        "discount": "0.00",
        "total_amount": "99.99",
        "amount_paid": "0.00",
        "payment_method": null,
        "payment_status": "unpaid",
        "amount_due": 99.99,
        "notes": null,
        "lat": "5.667783",
        "lng": "-0.166718",
        "address": "MR9M+376, Madina",
        "created_at": "2025-05-15T16:50:11.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Get Cart Summary
### Method: GET
>```
>{{baseurl}}/api/v1/users/cart
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

```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Cart retrieved successfully",
    "data": {
        "id": 1,
        "items": [
            {
                "id": 2,
                "cart_id": 1,
                "product": {
                    "id": 11,
                    "name": "Test Product",
                    "description": "This is a sample product description.",
                    "size": "Medium",
                    "images": [
                        {
                            "id": 1,
                            "image_url": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746985080/image/xusv3hpjnofc9wzi0kzl.jpg",
                            "display_order": 1,
                            "is_primary": true
                        },
                        {
                            "id": 2,
                            "image_url": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746985085/image/mo0ccfcnbk6md749piy9.jpg",
                            "display_order": 2,
                            "is_primary": false
                        }
                    ],
                    "price": "99.99",
                    "currency": "GHS",
                    "width": "10.50",
                    "height": "15.00",
                    "weight": null,
                    "sku": "HOLAe040",
                    "cost_price": "50.00",
                    "selling_price": "120.00",
                    "slug": "test-product-e5c4cb32-0676-47d4-87a2-058fb3ee8d24",
                    "is_out_of_stock": 0,
                    "is_disabled": 0,
                    "rating_count": 0,
                    "rating": "0.00",
                    "is_favorite": false,
                    "created_at": "2025-05-11T17:37:53.000000Z"
                },
                "quantity": 2,
                "price": "99.99",
                "total": 199.98,
                "created_at": "2025-05-14T14:27:39.000000Z",
                "updated_at": "2025-05-14T14:29:52.000000Z"
            }
        ],
        "summary": {
            "subtotal": 0,
            "total_items": 2,
            "tax": 0,
            "shipping": 0,
            "total": 0
        },
        "created_at": "2025-05-14T12:03:49.000000Z",
        "updated_at": "2025-05-14T12:03:49.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Add to Cart
### Method: POST
>```
>{{baseurl}}/api/v1/users/cart
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
    "product_id" : 1,
    "quantity"  :  1
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Item added to cart successfully",
    "data": {
        "id": 1,
        "items": [
            {
                "id": 3,
                "cart_id": 1,
                "product": {
                    "id": 11,
                    "name": "Test Product",
                    "description": "This is a sample product description.",
                    "size": "Medium",
                    "images": [
                        {
                            "id": 1,
                            "image_url": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746985080/image/xusv3hpjnofc9wzi0kzl.jpg",
                            "display_order": 1,
                            "is_primary": true
                        },
                        {
                            "id": 2,
                            "image_url": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746985085/image/mo0ccfcnbk6md749piy9.jpg",
                            "display_order": 2,
                            "is_primary": false
                        }
                    ],
                    "price": "99.99",
                    "currency": "GHS",
                    "width": "10.50",
                    "height": "15.00",
                    "weight": null,
                    "sku": "HOLAe040",
                    "cost_price": "50.00",
                    "selling_price": "120.00",
                    "slug": "test-product-e5c4cb32-0676-47d4-87a2-058fb3ee8d24",
                    "is_out_of_stock": 0,
                    "is_disabled": 0,
                    "rating_count": 0,
                    "rating": "0.00",
                    "is_favorite": false,
                    "created_at": "2025-05-11T17:37:53.000000Z"
                },
                "quantity": 1,
                "price": "99.99",
                "total": 99.99,
                "created_at": "2025-05-14T14:41:09.000000Z",
                "updated_at": "2025-05-14T14:41:09.000000Z"
            }
        ],
        "summary": {
            "subtotal": 0,
            "total_items": 1,
            "tax": 0,
            "shipping": 0,
            "total": 0
        },
        "created_at": "2025-05-14T12:03:49.000000Z",
        "updated_at": "2025-05-14T12:03:49.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Update Cart
### Method: PATCH
>```
>{{baseurl}}/api/v1/users/cart/{cart_id}
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
    "product_id" : "",
    "quantity"   : 1
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "message": "Item updated successfully",
    "data": {
        "id": 1,
        "items": [
            {
                "id": 3,
                "cart_id": 1,
                "product": {
                    "id": 11,
                    "name": "Test Product",
                    "description": "This is a sample product description.",
                    "size": "Medium",
                    "images": [
                        {
                            "id": 1,
                            "image_url": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746985080/image/xusv3hpjnofc9wzi0kzl.jpg",
                            "display_order": 1,
                            "is_primary": true
                        },
                        {
                            "id": 2,
                            "image_url": "https://res.cloudinary.com/dfdz4coc9/image/upload/v1746985085/image/mo0ccfcnbk6md749piy9.jpg",
                            "display_order": 2,
                            "is_primary": false
                        }
                    ],
                    "price": "99.99",
                    "currency": "GHS",
                    "width": "10.50",
                    "height": "15.00",
                    "weight": null,
                    "sku": "HOLAe040",
                    "cost_price": "50.00",
                    "selling_price": "120.00",
                    "slug": "test-product-e5c4cb32-0676-47d4-87a2-058fb3ee8d24",
                    "is_out_of_stock": 0,
                    "is_disabled": 0,
                    "rating_count": 0,
                    "rating": "0.00",
                    "is_favorite": false,
                    "created_at": "2025-05-11T17:37:53.000000Z"
                },
                "quantity": 1,
                "price": "99.99",
                "total": 99.99,
                "created_at": "2025-05-14T14:41:09.000000Z",
                "updated_at": "2025-05-14T14:42:35.000000Z"
            }
        ],
        "summary": {
            "subtotal": 0,
            "total_items": 1,
            "tax": 0,
            "shipping": 0,
            "total": 0
        },
        "created_at": "2025-05-14T12:03:49.000000Z",
        "updated_at": "2025-05-14T12:03:49.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Remove Item
### Method: DELETE
>```
>{{baseurl}}/api/v1/users/cart/{cart_id}
>```
### Response: 200
```json
{
    "message": "Item removed successfully",
    "data": {
        "id": 1,
        "user_id": 1,
        "items": [],
        "summary": {
            "subtotal": 0,
            "total_items": 0,
            "tax": 0,
            "shipping": 0,
            "total": 0
        },
        "created_at": "2025-05-14T12:03:49.000000Z",
        "updated_at": "2025-05-14T12:03:49.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Clear
### Method: DELETE
>```
>{{baseurl}}/api/v1/users/cart
>```
### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 200
```json
{
    "success": true,
    "message": "Cart cleared",
    "data": {
        "id": 1,
        "items": [],
        "summary": {
            "subtotal": 0,
            "total_items": 0,
            "tax": 0,
            "shipping": 0,
            "total": 0
        },
        "created_at": "2025-05-14T12:03:49.000000Z",
        "updated_at": "2025-05-14T12:03:49.000000Z"
    }
}
```


⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃ ⁃

## End-point: Checkout
### Method: POST
>```
>{{baseurl}}/api/v1/users/cart/checkout
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
    "notes" : "", //nullable
    "address" : "MR9M+376, Madina", 
    "lat" : "5.667783160429038",
    "lng" : "-0.16671788712757957"
}
```

### 🔑 Authentication bearer

|Param|value|Type|
|---|---|---|
|token|{{usertoken}}|string|


### Response: 400
```json
{
    "message": "Order created successfully",
    "data": {
        "id": 4,
        "order_number": "20250515HNB97O",
        "status": "pending",
        "subtotal": "99.99",
        "tax": "0.00",
        "shipping_cost": "0.00",
        "discount": "0.00",
        "total_amount": "99.99",
        "amount_paid": "0.00",
        "payment_method": null,
        "payment_status": "unpaid",
        "amount_due": 99.99,
        "notes": null,
        "lat": "5.667783",
        "lng": "-0.166718",
        "address": "MR9M+376, Madina",
        "created_at": "2025-05-15T20:25:42.000000Z",
        "user": {
            "id": 2,
            "name": "Derrick Azaglo",
            "email": "de.azaglo@gmail.com",
            "phone": "+233549632604"
        },
        "order_group": {
            "id": 4,
            "created_at": "2025-05-15T20:25:42.000000Z"
        },
        "items": [
            {
                "id": 3,
                "quantity": 1,
                "price": null,
                "total": "0.00",
                "product": {
                    "id": 1,
                    "name": "Test Product",
                    "description": "This is a sample product description.",
                    "price": "99.99",
                    "image": null,
                    "sku": "HOLAe040"
                }
            }
        ]
    }
}
```

