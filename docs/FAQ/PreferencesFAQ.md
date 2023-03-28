# FAQ

## Preferences

1. What does UnderpaymentAllocation mean?
  
    A: Underpayments: 
      ALIGNDLN = Align delinquencies
      PRORTPASTDUE = Prorate by total past due amounts
      MOSTMPA = By most delinquent, then lowest MPA
      *Note: States might change the default.*\n\n\t\t**Default allocation method when customer has not saved an option*
  
2. What does OverpaymentAllocation mean?
  
    A: Overpayments:
      HIGHINTRT = Highest Interest Rate
      HIGHBAL = Highest current balance
      LOWBAL = Lowest current balance
      PRORTMPA = Prorate by MPA
      NONSUB = Unsub loan(s)
    If more than one loan meets has the same interest rate, the payment is applied to the loan without the subsidy. If there are no loans without a subsidy, the payment is prorated across those loans by MPA.
    *This is a FFELP/DL item only, this will not apply to Earnest.*

3. Is AdvanceDueDate the "PayDown" vs "PayAhead" option that we would allow the clients to toggle between?
  
    A: Yes. Values are "Y" or "N"
  
4. Is the API expecting "TRUE", "FALSE" as the value to be passed for each of these options?
  
    A: No. There are actual values. Preference Names: UnderpaymentAllocation, OverpaymentAllocation, AdvanceDueDate
