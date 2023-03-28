# FAQ

## Phones

1. Where do we get the AutoDialConsentReason value from?
  
    A: The API is expecting one of these "NoCustomerResponse, ConsentGiven, ConsentNotGiven, Litigation"
  
2. Would AutoDialConsent and TextConsent options cover all TCPA requirements?
  
    A: Processes need to be in place to use these values unless there is a legal reason why they don't have to be.
  
3. How do I only get "good" numbers?
  
    A: /phones/api/v1/persons/[personid]/phones?status=good
  
4. How do I only get the primary number?
  
    A: /phones/api/v1/persons/[personid]/phones?isPrimary=true
  
5. How can I get only certain types of phone numbers back?

    A: To only get "land" numbers, then <path>. 
To only get "cell" numbers, then <path>. And so on for each of the applicable types.
  
6. How do I only get work numbers?
  
    A: /phones/api/v1/persons/[personid]/phones?isWorkPhoneNumber=true
  
7. How many active phone numbers can be associated to a person?
  
    A: There is currently no limit to the number of active phone numbers a person can have associated to their account.
