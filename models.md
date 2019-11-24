# Models description

## User

Start with model inherited from Django user

## MerchantCategory

- mcc (Merchant category code) https://github.com/greggles/mcc-codes/blob/master/mcc_codes.json
- description

## Counterparty - can be user himself, another person, shop, bank etc.

## Subclasses of counterparty

- Person
- Shop
- Bank
- Employer

## Account

- name
- description - optional
- owner - Counterparty
- currency
- balance

## Transaction

- write_off_account
- write_on_account
- amount
- currency
- time
- is_completed

- type (visual attribute):
+ spending - choose your account to write off and a counterparty,
+ income - choose a counterparty and your account to refill,
+ transfer, loan obtain, loan repay, saving retain, saving replenishment (all identical) - choose two your accounts for transfer from one to another

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
