# FAQ

## Permissions

1. Fiserv accepts a Boolean (True/False) value for these fields : Email1098, EmailRegulatory, EmailNonRegulatory, EmailMarketing, PhoneMarketing, USPSMarketing, AffiliateShareMarketing
  1. How do I indicate to send correspondence electronically for a given permission code/type (i.e., Email1098)?

      A: Pass a TRUE value.

  
  2. How do I indicate to send correspondence via USPS for a given permission code/type (i.e., Email 1098)?

      A: Pass a FALSE value.
  
  3. Do all permission codes/types have to be set to the same value (i.e., all set to TRUE)?

      A: No, each permission code/type has its own value. You can set all codes/types to the same value or you can have a mix of TRUE and FALSE values.
  
2. Is Text marketing the same as "PhoneMarketing" in the API?
  
    A: No. (Text marketing is supported by the Phone API.)
