# Experiment 13: Role-Based Authorization

## Objective
Implement JWT-based authentication and role-based authorization (Admin vs User) in Node.js + Express + MongoDB.

## Steps
1. Setup Node.js project and install dependencies.
2. Create .env for PORT, MongoDB URI, and JWT secret.
3. Create User model with role field.
4. Implement JWT authentication middleware.
5. Implement role-based authorization middleware.
6. Create routes: /register, /login, /profile (user), /admin (admin).
7. Test using Postman:
   - Register user/admin
   - Login to get JWT token
   - Access /profile with any token
   - Access /admin with admin token only

## Screenshots
*App Screenshot*:

![App Screenshot](public/ss1.png)

![App Screenshot](public/ss2.png)


## Notes
- JWT token expires in 1 hour
- Only admin users can access /admin
- Regular users trying to access /admin get 403 Forbidden
