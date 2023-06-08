# API Spec

## Create Product

Request: 
- Method: POST
- Endpoint : `/api/products`
- Header: 
    - Content Type: application/json
    - Accept: application/json
- Body: 
```json
{
  "id" : "string, unique",
  "name" : "string",
  "price" : "long",
  "quantity" : "integer"
}
```

Response: 
```json
{
  "code": "number",
  "status": "string",
  "data": {
    "id": "string, unique",
    "name": "string",
    "price": "long",
    "quantity": "integer"
  }
}
```

## Get Product
- Method: GET
- Endpoint : `/api/products{id_product}`
- Header:
  - Accept: application/json

Response:
```json
{
  "code": "number",
  "status": "string",
  "data": {
    "id": "string, unique",
    "name": "string",
    "price": "long",
    "quantity": "integer"
  }
}
```

## Update Product
- Method: PUT
- Endpoint : `/api/products{id_product}`
- Header:
  - Content Type: application/json
  - Accept: application/json
- Body:
```json
{
  "code": "number",
  "status": "string",
  "data": {
    "id": "string, unique",
    "name": "string",
    "price": "long",
    "quantity": "integer"
  }
}
```

Response:
```json
{
  "code": "number",
  "status": "string",
  "data": {
    "id": "string, unique",
    "name": "string",
    "price": "long",
    "quantity": "integer"
  }
}
```

## List Product
- Method: GET
- Endpoint : `/api/products`
- Header:
  - Accept: application/json
- Query Param:
  - size: number,
  - page: number
- Body:
```json
{
  "code": "number",
  "status": "string",
  "data": [
    {
      "id": "string, unique",
      "name": "string",
      "price": "long",
      "quantity": "integer"
    },
    {
      "id": "string, unique",
      "name": "string",
      "price": "long",
      "quantity": "integer"
    }
  ]
}
```

Response:
```json
{
  "code": "number",
  "status": "string",
  "data": {
    "id": "string, unique",
    "name": "string",
    "price": "long",
    "quantity": "integer"
  }
}
```

## Delete Product
- Method: DELETE
- Endpoint : `/api/products{id_product}`
- Header:
  - Accept: application/json

Response:
```json
{
  "code": "number",
  "status": "string"
}