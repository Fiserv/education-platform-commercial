# FAQ

## Addresses


1. How do I only get certain types of addresses returned?

    A: To get only the address designated as primary, use /addresses/api/v1/persons/[personid]/addresses?isPrimary=true
    
    Otherwise, set isPrimary=false or leave isPrimary parameter off altogether to have all active addresses associated to the person returned.

2. Are addresses validated?

    A: Client is responsible for executing any validation of their choosing prior to calling the API and when calling the API ensuring adherence to the schema                  definition. The API will validate required fields are present and any field value provided aligns to the field definition. Once the address is stored on the              system of record it will be run through a process for standardizing delivery addresses. 
