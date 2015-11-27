Problem 3
===
Create a Rails app which uses **Devise** gem for authentication. But instead of using database, use an API for authentication.

##### API application
routes

1. **POST: /v1/register**

   Params: name, email_id, password

   Returns:  
   on Success  
   ```
   {:status => "success", :user_id => <id>}
   ```  
   on Failure  
   ```
   {:status => "failed", :reason => ""}
   ```  

2. **POST: /v1/authenticate**

   Params: email_id, password

   Returns:  
   on Success  
   ```
   {:status => "success"}
   ```  
   on Failure  
   ```
   {:status => "failed", :reason => ""}   
   ```  

##### Web application

Has following things  

1. Sign up page (register via Devise using /v1/register API end point)
2. Sign in page (authenticate via Devise using /v1/authenticate end point)
3. A dummy home page. This should be shown if sign in (or sign up) is successful. This page should not be accessible without a valid session
