# spring-boot2-oauth2

This is an example project for integrating OAuth2

Run the project using `./mvnw spring-boot:run`


Credits to the original authors and the people who discussed the solution at 
https://github.com/spring-projects/spring-boot/issues/12346


$ curl -X POST http://localhost:8000/auth/oauth/token -H 'authorization: Basic YWNtZTpzZWNyZXQ=' -H 'cache-control: no-cache' -H 'content-type: multipart/form-data' -F username=john@example.com -F password=password -F grant_type=password
{"access_token":"8f6d7f22-db8e-4799-b45a-c856bc9c766e","token_type":"bearer","refresh_token":"d622e5fa-78c4-45f9-8396-2ab50b4cdff6","expires_in":3599,"scope":"read write"}
