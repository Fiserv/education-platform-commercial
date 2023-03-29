# FAQ

## Phones
  
1. How do I only get "good" numbers?
  
    A: /phones/api/v1/persons/[personid]/phones?status=good
  
2. How do I only get the primary number?
  
    A: /phones/api/v1/persons/[personid]/phones?isPrimary=true
  
3. How can I get only certain types of phone numbers back?

    A: To only get "land" numbers, then <path>. 
To only get "cell" numbers, then <path>. And so on for each of the applicable types.
  
4. How do I only get work numbers?
  
    A: /phones/api/v1/persons/[personid]/phones?isWorkPhoneNumber=true
  
5. How many active phone numbers can be associated to a person?
  
    A: There is currently no limit to the number of active phone numbers a person can have associated to their account.
