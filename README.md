# mok-api0.1
 mok  api 
Here's a **README.md** file for your **Mock API** section:

```markdown
# Mock API Documentation

## Overview
This is a simple mock API server for testing and development purposes. It simulates REST API endpoints with realistic responses.

## Base URL
```
http://localhost:3000/api
```

## Endpoints

### GET /users
Returns a list of all users.

**Response:**
```json
{
  "success": true,
  "data": [
    { "id": 1, "name": "Dushyant Saket", "email": "dushyant@example.com" },
    { "id": 2, "name": "John Doe", "email": "john@example.com" }
  ]
}
```

### GET /users/:id
Returns a specific user by ID.

**Response:**
```json
{
  "success": true,
  "data": { "id": 1, "name": "Dushyant Saket", "email": "dushyant@example.com" }
}
```

### POST /users
Creates a new user.

**Request Body:**
```json
{ "name": "New User", "email": "new@example.com" }
```

**Response:**
```json
{
  "success": true,
  "message": "User created",
  "userId": 3
}
```

### PUT /users/:id
Updates an existing user.

**Response:**
```json
{
  "success": true,
  "message": "User updated successfully"
}
```

### DELETE /users/:id
Deletes a user.

**Response:**
```json
{
  "success": true,
  "message": "User deleted successfully"
}
```

## Error Response Format
```json
{
  "success": false,
  "error": "User not found",
  "code": 404
}
```

## How to Run

### Using JSON Server
```bash
npm install -g json-server
json-server --watch db.json --port 3000
```

### Sample `db.json`
```json
{
  "users": [
    { "id": 1, "name": "Dushyant Saket", "email": "dushyant@example.com" }
  ]
}
```

## Version
**v0.1** - Initial release
```

Would you like me to adjust this for your specific needs? 
