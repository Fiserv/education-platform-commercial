# FAQ

## Phones
  
1. How can I get only certain phone numbers back?
    
    A: Each phone number contains optional attributes that can be used to customize the result set to the sub-set of active phone numbers you are interested in. Leaving these attributes off altogether will result in all active phone numbers associated to the person being returned. Example use cases include:
    
	  To get only “good” (i.e., not bad or disconnected) phone numbers, use /phones/api/v1/persons/[personid]/phones?status=good
  
    To get the phone number the person has designated as the primary number, use /phones/api/v1/persons/[personid]/phones?isPrimary=true

    To get only phone numbers the person has designated as work numbers, use /phones/api/v1/persons/[personid]/phones?isWorkPhoneNumber=true

    To get only cell (aka mobile) phone numbers, use /phones/api/v1/persons/[personid]/phones?Type=cell

2. How many active phone numbers can be associated to a person?
  
    A: There is currently no limit to the number of active phone numbers a person can have associated to their account.
