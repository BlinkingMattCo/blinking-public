# API Documentation

## Overview

This document describes the API endpoints for the Blinking Public service.

## Authentication

All API requests require authentication using Bearer tokens.

```bash
curl -H "Authorization: Bearer YOUR_TOKEN" https://api.example.com/endpoint
```

## Endpoints

### User Management

#### GET /api/users

Retrieve a list of users.

**Response:**
```json
{
  "users": [
    {
      "id": 1,
      "username": "john_doe",
      "email": "john@example.com"
    }
  ]
}
```

#### POST /api/users

Create a new user.

**Request:**
```json
{
  "username": "jane_doe",
  "email": "jane@example.com",
  "password": "secure_password"
}
```

## Error Codes

- `400` - Bad Request
- `401` - Unauthorized
- `404` - Not Found
- `500` - Internal Server Error
