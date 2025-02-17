## Payments Team Call Takeaways:

Payment status/payment code is a static field and can be replicated as in Oracle DB.
Any additions to status or code can be accommodated as per the Payments team.
Discovery on payments and data sources is still ongoing, with more details to follow.
## Post-Call Work Done:

Analyzed gcms_funds_transfer_details table.
Examined details related to wire transfer payments and beneficiary information.
Reviewed data structure in Oracle DB for relevant insights.

## Final Adjustments & Considerations
SUN_ID and BRANCH_ID should be mandatory fields for all transactions.
Ensure PAYMENT_AMOUNT adheres to 15-character formatting.
Link PARTY_1 and PARTY_2 based on PARTY_ID and PARTY_BRANCH_ID.
Store Beneficiary details for the same customer to avoid duplication.
Implement a new audit table to track modifications in payment and beneficiary data.
