# User Service using Spring Authorization Server and JWT (In Memory)

## Problem Statement

You are working on a project that requires you to create a user service. Implement the Spring Authorization Server to authenticate users and generate JWT tokens. 

## Requirements
1. Use Spring Authorization Server to create a user service using documentation: https://docs.spring.io/spring-authorization-server/reference/getting-started.html
2. Make the required changes to SecurityConfig.java to configure the Authorization Server.
3. Add Postman application as a client with clientId: `oidc-client` and clientSecret: `secret` with the required scopes.
4. Use appropriate redirect URIs to redirect the user to the client(Postman) after login.
5. Add a user with username: `user` and password: `password` with the required roles to create the user and UserDetailsService to load the user.
6. For testing, use Authorization function available in Postman to get the JWT token by providing the required details like Client ID, Client Secret and Scope.
7. Use the following endpoints in Postman to authenticate the user and generate the JWT token:
    - `/oauth/authorize`: This endpoint should authenticate the user and generate the JWT token.
    - `/oauth/token`: This endpoint should generate the JWT token.
8. Clicking on "Get New Access Token" should redirect the user to the login page where the user can enter the username and password to authenticate. Once authenticated, the user should be redirected to the client(Postman) with the JWT token.
