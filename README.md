# Planning

## Core features to implement

1. Easy receipt scan and parse. Need to parse store name, date and total amount. Tried https://pypi.org/project/pytesseract/ a bit. Needs some way to be smart about results parsing. Also some good way to scan receipts instead of making photos.
1. Bank API integration. First step - Monobank API https://api.monobank.ua/docs/. When some test version is ready need to obtain corporate API permission.
1. Possible integrations with some stores API - low chance to have that.
1. Manual data input.
1. Break down entered spending into several smaller ones.
1. Enter your existing property value and set amortization scheme.
1. Analyze spendings over time and make predictions.
1. Set planned spendings and compare planned and actual spendings.
1. Set and track goals or hard limits per category.
1. Reminders for payments.
1. Shopping lists.
1. Google maps integration to get businesses.
1. Loans and deposists calculators.
1. Badges, rewards.
1. Offline mode in the apps in the future.
1. SECURITY???

## Technologies

- Django backend at the start
- React web client + React native apps in the future
- GraphQL + fetching and backend libraries
- Material UI for prototyping
- Deploy to Heroku

## Rough roadmap

1. Essential features:
- Accounts (cash, bank, saving, loan etc.)
- Transactions
- Categories
- Polling data from Monobank
- Basic graphs
