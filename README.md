# laravel-api-auth

1. composer install
2. php artisan migrate
3. php artisan serve


API (with token base authentication)
 => check working
 GET http://localhost:8000/api/public (Postman)
 
 => login
POST http://localhost:8000/api/login (Postman)
Content-Type: application/json
{
    "email": "test@example.com",
    "password": "password"
}

=> protected
GET http://localhost:8000/api/protected (Postman)
Authorization: Bearer YOUR_TOKEN_HERE 

=> logout
POST http://localhost:8000/api/logout (Postman)
Authorization: Bearer YOUR_TOKEN_HERE
