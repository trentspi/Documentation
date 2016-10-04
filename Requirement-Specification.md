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

## Credentials
- unique username
- text password

## Authentication
- Should use JSON Web Tokens (JWT)
- Should use BCrypt to hash user password

### Authentication Process
- Login
  - User enters credentials
  - System validates user credentials
  - System returns JWT
  - User uses JWT to access authenticated routes
- Logout
  - Expire users JWT

# Calendar System Requirements
## User views
- Should be able to view a single Month
- Should be able to view a single Day
- Should be able to switch between Months
- Should be able to switch between Days

## Tasks
- Should be able to create Tasks
- Should be able to remove Tasks
- Should be able to update Tasks
- Should be able to delete Tasks
- Tasks must be associated with an individual Day
- Should be able to change a Tasks' Day