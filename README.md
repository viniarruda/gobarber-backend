# GoBarber Api

- ORM
- Migration
- Seeds
- MVC
- Sequelize
- Postbird
- JWT
- Bcrypt
- MD5Online
- Nodemailer
- Mailtrap
- Redis for queue
- Beequeue
- [Sentry](https://sentry.io) for errors
- Youch

-eslint
`yarn eslint --fix src --ext .js`

## Docker

`docker ps`

`docker start database`

`docker run --name mongobarber -p 27017:27017 -d -t mongo`

`docker run --name redisbarber -p 6379:6379 -d -t redis:alpine`

`docker ps` // All Docker containers run

`docker ps -a` // All Docker containers

### Sequelize

`yarn sequelize db:migrate`

`yarn sequelize db:migrate:undo` // Last migrate

`yarn sequelize db:migrate:undo:all` // All migrations

### Helpers

- [Api pattern](https://docs.nestjs.com/recipes/cqrs)
- [Api pattern](https://medium.com/laraveltips/voc%C3%AA-entende-repository-pattern-voc%C3%AA-est%C3%A1-certo-disso-d739ecaf544e)

```
{
	"name": "Customer",
	"email": "customer@email.com",
	"password": "test123"
},
{
	"name": "Professional",
	"email": "professional@email.com",
	"password": "test123",
	"provider": true
}
```

### NOTES

Separe queue because is better to run in other instance
