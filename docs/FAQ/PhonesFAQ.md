# FAQ

## Phones

1. Where do we get the AutoDialConsentReason value from?
  
    A: The API is expecting one of these "NoCustomerResponse, ConsentGiven, ConsentNotGiven, Litigation"
  
2. For TextConsent, are the acceptable values TRUE, FALSE?
  
    A: The acceptable values are "true" or "false"
  
3. Would AutoDialConsent and TextConsent options cover all TCPA requirements?
  
    A: Processes need to be in place to use these values unless there is a legal reason why they don't have to be.
  
4. Where do we get the PhoneStatus of "Good, Bad, Disconnect"?
  
    A: The current values will be returned from the GET action of the Phones API
  
5. How do I only get "good" numbers?
  
    A: /phones/api/v1/persons/[personid]/phones?status=good
  
6. How do I only get the primary number?
  
    A: /phones/api/v1/persons/[personid]/phones?isPrimary=true
  
7. How do I only get "land" numbers? 
  
    A: /phones/api/v1/persons/[personid]/phones?Type=Land\n\n\t 
  *NOTE: Other phone type filter options: Cell, Land, Wireless, Pager, Fax, Foreign*
  
8. How do I only get work numbers?
  
    A: /phones/api/v1/persons/[personid]/phones?isWorkPhoneNumber=true
  
9. How many active phone numbers can be stored for the customer?
  
    A: Unlimited
