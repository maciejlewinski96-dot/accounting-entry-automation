# Automation Logic

The automation bot processes recurring journal entry requests provided in CSV format.

## Processing Steps

1. Bot reads the CSV input file.
2. File structure is validated.
3. Mandatory fields are checked.
4. Posting data is mapped to SAP journal entry structure.
5. Bot logs into SAP.
6. Journal entries are posted automatically.

## Validation Rules

Before posting, the bot verifies:

- posting date
- account number
- amount format
- currency code
- mandatory fields

## Exception Handling

If validation fails:

- posting is stopped
- error notification email is generated
- analyst reviews the issue

Only valid records proceed to SAP posting.
