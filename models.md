# Models description

## User

Start with model inherited from Django user

## AccountCategory

- mcc (Merchant category code) https://github.com/greggles/mcc-codes/blob/master/mcc_codes.json
- description

## Account

- name
- description - optional
- is_active (or passive)
- owner - Counterparty
- is_display - whether to show it in balance
- balance

## Counterparty - can be user himself, another person, shop, bank etc.

## Subclasses of counterparty

- Person
- Shop
- Bank

## Transaction

- debit_account
- credit_account
- amount
- currency
- time

### Monobank API response example:

```
{
  "id": "OYSlUeil8FXRDrE",
  "time": 1572530266,
  "description": "Uber",
  "mcc": 4121,
  "amount": -435,
  "operationAmount": -435,
  "currencyCode": 980,
  "commissionRate": 0,
  "cashbackAmount": 0,
  "balance": 2034497,
  "hold": false
}
```
