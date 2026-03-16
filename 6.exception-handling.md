# Exception Handling

The automation solution was designed to process standard recurring journal entries.  
However, certain scenarios required manual intervention.

## Typical Error Scenarios

Possible issues detected during validation:

- missing mandatory fields in CSV file
- incorrect account numbers
- invalid currency or amount format
- inconsistent posting structure

## Error Handling Logic

If an issue is detected:

1. The bot stops the posting process.
2. An automated email notification is sent to the finance analyst.
3. The email contains a short description of the detected issue.

## Analyst Action

After receiving the notification the analyst can:

- correct the CSV input file and resubmit it for processing, or
- perform manual posting in SAP if required.
