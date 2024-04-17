# Validation and security 

## Skills

- User data model and profiles 
- Validation with Bean Validation 
  - Annotations 
  - Customizing the HTTP response 
  - Custom validations with database access 
- Authentication and authorization 
  - Spring Security 
  - OAuth 2.0 
  - JWT Token 
  - Route authorization by profile 
- Postman tips 
- Environment variables in the project with coalescence

## TDD task

Implement the necessary features for the project tests to pass: https://github.com/devsuperior/bds04

This is a system of events and cities with an N-1 relationship between them:

![Figma](https://github.com/SofiaMFonseca/assets/blob/main/bds04/conceptual-model-bds04.png)

In this system, only the read routes (GET) of events and cities are public (no login required). CLIENT users can also POST new events. Other accesses are allowed only to ADMIN users.

### City Validations:

- Name cannot be empty 

### Event Validations: 

- Name cannot be empty 
- Date cannot be before the present moment 
- City cannot be null 
