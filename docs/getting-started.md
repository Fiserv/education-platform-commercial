# Getting Started

## Get Your Credentials

Reach out to us {contact info here?} to get your credentials to start calling our APIs.

## Calling APIs

### Initial Setup

First, you will need to go into settings and turn off "SSL Certificate Verification".

![SSLCert](/assets/images/Getting_Started/SSLCert_Setting.png)

If using Postman, you can download the Postman collection from the API page. 

If using a tool other than postman or you are creating a postman request manually, see below for instructions.

### Authorizations Setup

Each API call will first start with a call to the Authorizations API. Use the following information:

- Input the Authorizations endpoint and make it a POST method
- Encoding is x-www-form-urlencoded

Ensure your body has properties for:
 - grant_type
 - client_id
 - client_secret

In Postman this looks like:

![AuthorizationsSetup](/assets/images/Authorization_Body.jpg)

Once you send the request you will receive a response with a bearer token. This token will be used to make calls to the other APIs.

In Postman this looks like:

![AuthorizationsToken](/assets/images/Authorization_Token.png)

###All Other APIs Setup

Now that you have your token you can call any other API. To create the request manually do the following:

- Create a new request using the endpoint/method desired (info can be found in the API Explorer)
- Use the bearer token that was generated in the Authorizations response in your authorization header
- Update the "Body" as needed, based on the API you are calling

- Click "send" when ready

In Postman this looks like:

![APISetup](/assets/images/Getting_Started/API_Setup.png "API Setup")
![APIBody](/assets/images/Getting_Started/API_Body.jpg)

Note: If you get a 401 Unauthorized, make sure your token is correct and hasn't expired. Call the Authorizations API again to get a new token, as needed.



 
