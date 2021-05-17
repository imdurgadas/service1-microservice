
# Swagger Petstore

This is a sample server Petstore server.  You can find out more about     Swagger at [http://swagger.io](http://swagger.io) or on [irc.freenode.net, #swagger](http://swagger.io/irc/).      For this sample, you can use the api key `special-key` to test the authorization     filters.

## Indices

* [pet](#pet)

  * [Add a new pet to the store](#1-add-a-new-pet-to-the-store)
  * [Deletes a pet](#2-deletes-a-pet)
  * [Find pet by ID](#3-find-pet-by-id)
  * [Finds Pets by status](#4-finds-pets-by-status)
  * [Finds Pets by tags](#5-finds-pets-by-tags)
  * [Update an existing pet](#6-update-an-existing-pet)
  * [Updates a pet in the store with form data](#7-updates-a-pet-in-the-store-with-form-data)
  * [uploads an image](#8-uploads-an-image)

* [store](#store)

  * [Delete purchase order by ID](#1-delete-purchase-order-by-id)
  * [Find purchase order by ID](#2-find-purchase-order-by-id)
  * [Place an order for a pet](#3-place-an-order-for-a-pet)
  * [Returns pet inventories by status](#4-returns-pet-inventories-by-status)

* [user](#user)

  * [Create user](#1-create-user)
  * [Creates list of users with given input array](#2-creates-list-of-users-with-given-input-array)
  * [Creates list of users with given input array](#3-creates-list-of-users-with-given-input-array)
  * [Delete user](#4-delete-user)
  * [Get user by user name](#5-get-user-by-user-name)
  * [Logs out current logged in user session](#6-logs-out-current-logged-in-user-session)
  * [Logs user into the system](#7-logs-user-into-the-system)
  * [Updated user](#8-updated-user)


--------


## pet
Folder for pet



### 1. Add a new pet to the store



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: https://petstore.swagger.io/v2/pet
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |
| Content-Type | application/json |  |



***Body:***

```js        
Pet object that needs to be added to the store
```



### 2. Deletes a pet



***Endpoint:***

```bash
Method: DELETE
Type: FORMDATA
URL: https://petstore.swagger.io/v2/pet/:petId
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |
| api_key | {{api_key}} |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| petId | {{petId}} |  |



### 3. Find pet by ID


Returns a single pet


***Endpoint:***

```bash
Method: GET
Type: 
URL: https://petstore.swagger.io/v2/pet/:petId
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| petId | {{petId}} |  |



### 4. Finds Pets by status


Multiple status values can be provided with comma separated strings


***Endpoint:***

```bash
Method: GET
Type: 
URL: https://petstore.swagger.io/v2/pet/findByStatus
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| status | {{status}} |  |



### 5. Finds Pets by tags


Muliple tags can be provided with comma separated strings. Use         tag1, tag2, tag3 for testing.


***Endpoint:***

```bash
Method: GET
Type: 
URL: https://petstore.swagger.io/v2/pet/findByTags
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| tags | {{tags}} |  |



### 6. Update an existing pet



***Endpoint:***

```bash
Method: PUT
Type: RAW
URL: https://petstore.swagger.io/v2/pet
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |
| Content-Type | application/json |  |



***Body:***

```js        
Pet object that needs to be added to the store
```



### 7. Updates a pet in the store with form data



***Endpoint:***

```bash
Method: POST
Type: URLENCODED
URL: https://petstore.swagger.io/v2/pet/:petId
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |
| Content-Type | application/x-www-form-urlencoded |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| petId | {{petId}} |  |



***Body:***


| Key | Value | Description |
| --- | ------|-------------|
| name | {{name}} |  |
| status | {{status}} |  |



### 8. uploads an image



***Endpoint:***

```bash
Method: POST
Type: FORMDATA
URL: https://petstore.swagger.io/v2/pet/:petId/uploadImage
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/json |  |
| Content-Type | multipart/form-data |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| petId | {{petId}} |  |



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| additionalMetadata | {{additionalMetadata}} |  |
| file | {{file}} |  |



## store
Folder for store



### 1. Delete purchase order by ID


For valid response try integer IDs with positive integer value.         Negative or non-integer values will generate API errors


***Endpoint:***

```bash
Method: DELETE
Type: FORMDATA
URL: https://petstore.swagger.io/v2/store/order/:orderId
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| orderId | {{orderId}} |  |



### 2. Find purchase order by ID


For valid response try integer IDs with value >= 1 and <= 10.         Other values will generated exceptions


***Endpoint:***

```bash
Method: GET
Type: 
URL: https://petstore.swagger.io/v2/store/order/:orderId
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| orderId | {{orderId}} |  |



### 3. Place an order for a pet



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: https://petstore.swagger.io/v2/store/order
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***Body:***

```js        
order placed for purchasing the pet
```



### 4. Returns pet inventories by status


Returns a map of status codes to quantities


***Endpoint:***

```bash
Method: GET
Type: 
URL: https://petstore.swagger.io/v2/store/inventory
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/json |  |



## user
Folder for user



### 1. Create user


This can only be done by the logged in user.


***Endpoint:***

```bash
Method: POST
Type: RAW
URL: https://petstore.swagger.io/v2/user
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***Body:***

```js        
Created user object
```



### 2. Creates list of users with given input array



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: https://petstore.swagger.io/v2/user/createWithArray
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***Body:***

```js        
List of user object
```



### 3. Creates list of users with given input array



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: https://petstore.swagger.io/v2/user/createWithList
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***Body:***

```js        
List of user object
```



### 4. Delete user


This can only be done by the logged in user.


***Endpoint:***

```bash
Method: DELETE
Type: FORMDATA
URL: https://petstore.swagger.io/v2/user/:username
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| username | {{username}} |  |



### 5. Get user by user name



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://petstore.swagger.io/v2/user/:username
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| username | {{username}} |  |



### 6. Logs out current logged in user session



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://petstore.swagger.io/v2/user/logout
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



### 7. Logs user into the system



***Endpoint:***

```bash
Method: GET
Type: 
URL: https://petstore.swagger.io/v2/user/login
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| username | {{username}} |  |
| password | {{password}} |  |



### 8. Updated user


This can only be done by the logged in user.


***Endpoint:***

```bash
Method: PUT
Type: RAW
URL: https://petstore.swagger.io/v2/user/:username
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Accept | application/xml, application/json |  |



***URL variables:***

| Key | Value | Description |
| --- | ------|-------------|
| username | {{username}} |  |



***Body:***

```js        
Updated user object
```



---
[Back to top](#swagger-petstore)
> Made with &#9829; by [thedevsaddam](https://github.com/thedevsaddam) | Generated at: 2021-05-17 21:36:40 by [docgen](https://github.com/thedevsaddam/docgen)
