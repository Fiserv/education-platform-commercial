# Getting Started

### Get Your Credentials

Reach out to us {contact info here?} to get your credentials to start calling our APIs.

### Calling APIs

##### Authorizations

All API calls will first start with Authorizations. This will provide you with a JSON token to call any of our other APIs with.

##### Subsequent Calls

Please refer to the documentation here on what's needed to call other APIs


### Try it Out Using Postman

First, you will need to go into settings and turn off "SSL Certificate Verification"

![SSLCert](/assests/images/Getting_Started/SSLCert_Setting.png)

Now you can either download the Postman collection from the API page, or create a new request manually. If creatin a new request, see below for instructions.

##### Authorizations

As stated above, any API call will first start with Authorizations. To set it up do the following.

- Update the "Body"
    - Select "x-www-form-urlencoded"
    - Update with three keys: grant_type, client_id, client_secret and assign them the appropriate values.

- Input the Authorizations endpoint and make it a POST method

![AuthorizationsSetup](/assets/images/Getting_Started/Authorization_Body.png)

Send the request and grab the token from the response. This will be used for calls in other APIs

![AuthorizationsToken](/assets/images/Getting_Started/Authorization_Token.png)

##### Other APIs

Now that you have your token you can call any other API. To create the request manually do the following.

- Create a new request using the endpoint/method desired (info can be found in the API docs)
- Under the "Authorization" tab select "Bearer Token" and use the token that was generated in the Authorizations response

![APISetup](/assets/images/Getting_Started/API_Setup.png)

- Update the "Body" if/as needed, refer to API documentation

![APIBody](/assets/images/Getting_Started/API_Body.png)

- Click "send" when ready

Note: If you get an 401 Unauthorized, make sure your token is correct and hasn't expired. Call Authorizations again and grab the new token if needed.



 
