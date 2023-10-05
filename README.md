# Products-API-v2

This API is designed to manage products, allowing you to Create, Read, Update, and Delete product information.

## Base URL

All requests should be made to:
https://zzz02ohgi4.execute-api.eu-north-1.amazonaws.com/dev

## Common Headers

For all requests:

- **User-Agent**: `insomnia/8.1.0`

## Endpoints

### 1. Read - All products

- **Method**: GET
- **Endpoint**: `/products`
- **Headers**:
  - **User-Agent**: `insomnia/8.1.0`

### 2. Create an Item

- **Method**: POST
- **Endpoint**: `/product`
- **Headers**:
  - **Content-Type**: `application/json`
  - **authorizationToken**: `allow`
  - **User-Agent**: `insomnia/8.1.0`
- **Body**:

```json
{
  "price": "3299",
  "itemName": "Apple Airpods Pro 2nd Gen"
}
```

#### 3. **Read - {itemId}**

- **Method**: GET
- **Endpoint**: `/product/{itemId}`
- **Headers**:
  - **User-Agent**: `insomnia/8.1.0`

---

#### 4. **Update**

- **Method**: PUT
- **Endpoint**: `/product/{itemId}`
- **Headers**:
  - **Content-Type**: `application/json`
  - **authorizationToken**: `allow`
  - **User-Agent**: `insomnia/8.1.0`

**Request Body**:

```json
{
  "price": "22999",
  "itemName": "Apple Macbook Air 15 inch - Updated"
}
```

#### 5. **Delete**

- **Method**: DELETE
- **Endpoint**: `/product/{itemId}`
- **Headers**:
  - **authorizationToken**: `allow`
  - **User-Agent**: `insomnia/8.1.0`

`{itemId}` in the endpoint paths is replaced with the specific product ID when making a request.
