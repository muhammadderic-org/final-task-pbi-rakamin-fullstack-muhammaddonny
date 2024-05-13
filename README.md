# final-task-pbi-rakamin-fullstack-muhammaddonny

# About Photo Manager API

Creating a Backend API with Golang for my first project introduces me to essential web development concepts like routing, handling HTTP requests, and database integration

## Functionalities

1. User registration and login + User validation input
2. User authorization using JWT (for accessing photo manager)
3. Basic photo manager (upload, edit, and delete)

## Usage Guidelines

The database used is MySQL, and Thunder Client extension in VSCode to make a request to the API

This is the list of routes that you can use:

// User <br>
Register: http://localhost:9090/users/register (POST)<br>
Login: http://localhost:9090/users/login (POST)<br>
Update User: http://localhost:9090/users/:id (PUT)<br>
Delete User: http://localhost:9090/users/:id (DELETE)<br>
Logout: http://localhost:9090/users/logout (POST)<br>

// Photo<br>
Get Photos: http://localhost:9090/photos (GET)<br>
Create Photo: http://localhost:9090/photos (POST)<br>
Update Photo: http://localhost:9090/photos/:id (PUT)<br>
DELETE Photo: http://localhost:9090/photos/:id (DELETE)<br>

When using POST method, you can parse some data in JSON format. For example, you can write the data like this for registering a new user:<br>
{<br>
&nbsp;&nbsp;&nbsp;&nbsp;"username": "johndoe",<br>
&nbsp;&nbsp;&nbsp;&nbsp;"email": "johndoe@gmail.com",<br>
&nbsp;&nbsp;&nbsp;&nbsp;"password": "123456"<br>
}

## Depedencies

- [gin](https://github.com/gin-gonic/gin): A web framework that simplifies routing, middleware, and request handling in Go applications.
- [gorm](https://github.com/go-gorm/gorm): An Object-Relational Mapping (ORM) library that helps interact with databases in a structured and efficient way.
- [go-mysql driver](https://github.com/go-sql-driver/mysql): A MySQL driver for Go that enables communication between Go applications and MySQL databases, facilitating database operations.
- [jwt-go](https://github.com/golang-jwt/jwt): A library for JSON Web Tokens (JWT) in Go, useful for implementing secure authentication and authorization mechanisms.
- [bcrypt](https://pkg.go.dev/golang.org/x/crypto/bcrypt): A library for hashing passwords securely, commonly used for user authentication systems.

## References

I greatly appreciate the support from the forum community and tutorial creators, as they have significantly contributed to enhancing my understanding of Golang. For newcomers to Golang, I highly recommend exploring these valuable resources for an accelerated learning experience.

- [Go Getting Started](https://go.dev/doc/tutorial/getting-started)
- [Gin Documentation](https://gin-gonic.com/docs/)
- [Gorm Documentation](https://gorm.io/index.html)