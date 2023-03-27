# FAQ

## Addresses API

1. Where do we get the LocationCode value from?/n
  A: The API is expecting one of these "SCHOOL, HOME, WORK"

2. How do I only get the primary address?
  A: /addresses/api/v1/persons/[personid]/addresses?isPrimary=true

3. Are addresses validated?
  A: There is internal validation run, but as long as all required fields are present it will be stored
