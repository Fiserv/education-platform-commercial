# FAQ

## Permissions

1. Fiserv accepts a Boolean (True/False) value for these fields : Email1098, EmailRegulatory, EmailNonRegulatory, EmailMarketing, PhoneMarketing, USPSMarketing, AffiliateShareMarketing
  1. If Paperless is selected, we would pass TRUE for the fields "Email1098, EmailRegulatory, EmailNonRegulatory
    
      A: "true" should be passed.
  
  2. If Paper is selected, we would pass FALSE for the fields \"Email1098, EmailRegulatory, EmailNonRegulatory"
    
      A: "false" should be passed.
  
  3. When we make a GET call on the Permissions API, would we always get back all TRUE (or all FALSE) for Email1098, EmailRegulatory, EmailNonRegulatory? And not a mix of TRUE and FALSE values?
    
      A:  Whatever the values are would be returned.  (That could be a mix of values, "true" or "false".)

2. What is AffiliateShareMarketing?
  
    A: This isn't used any more.
  
3. Is Text marketing the same as "PhoneMarketing" in the API?
  
    A: No. (Text marketing is supported by the Phone API.)
