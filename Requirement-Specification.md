# Calendar Application Requirements Specification
There will two different subsystems within our project

- Login System
- Calendar System

# Login System Requirements
## User
- Should be able to create a User
- Should be able to remove a User
- Should be able to update a User
- Should be able to delete a User

## Authentication
- Should use JSON Web Tokens (JWT)
- Should use BCrypt to hash user password

### Authentication Process
- Login:
  - User enters credentials
  - System validates user credentials
  - System returns JWT
  - User uses JWT to access authenticated routes
- Logout:
  - Expire users JWT