# REST API best practices

REST API for a CrossFit Training Application, in this application we'd like to create, read, update and delete WOD's (Workouts of the Day). This will help our users (that will be gym owners) come up with workout plans and maintain their own workouts inside a single application

## Start Project Command
```
npm install then npm run dev

```

## Architecture

Inside the Controller we'll be handling all stuff that is related to HTTP. That means we're dealing with requests and responses for our endpoints. Above that layer is also a little Router from Express that passes requests to the corresponding controller. 
 
The whole business logic will be in the Service Layer that exports certain services (methods) which are used by the controller. 
 
The third layer is the Data Access Layer where we'll be working with our Database. We'll be exporting some methods for certain database operations like creating a WOD that can be used by our Service Layer

![image](https://user-images.githubusercontent.com/31899798/184713570-1dcd68dc-65a8-4505-aa61-dcfe65ce551f.png)

### Reference

Example from https://www.freecodecamp.org/news/rest-api-design-best-practices-build-a-rest-api/

