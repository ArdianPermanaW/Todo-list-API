Routes
note: default port is 5000

Register:
http://localhost:5000/auth/register
Body
{
  "name": "Test",
  "email": "34324@example.com",
  "password": "password123"
}

Login:
http://localhost:5000/auth/login
Body
{
    "name": "Test User",
    "email": "test@example.com",
    "password": "password123"
}

Post todo item:
http://localhost:5000/todos
Header
key: Auth
Value: Bearer <key>
Body
{
  "title": "Test Test",
  "description": "Test",
  "dueDate": "2025-01-25T23:59:59.000Z"
}

Get todo item:
http://localhost:5000/todos?page=1&limit=10

Update todo item:
http://localhost:5000/todos/:id
Body
{
    "title": "Updated Todo Title",
    "description": "Updated description of the todo item.",
    "dueDate": "2025-01-25",
    "status": "completed"
}

Delete todo item:
http://localhost:5000/todos/:id




