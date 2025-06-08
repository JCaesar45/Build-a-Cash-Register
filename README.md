```markdown
# Cash Register Project

## Overview

This project simulates a simple cash register application that calculates change due to a customer based on the purchase price and cash provided. It handles multiple test cases including insufficient funds, exact payment, and returning correct change with available denominations.

---

## Features

- Displays purchase price dynamically.
- Accepts cash input from user.
- Calculates change due or alerts if customer cash is insufficient.
- Determines if cash in drawer (CID) can cover the change.
- Returns change in highest to lowest denominations.
- Handles exact payment with no change due.
- Shows status messages:
  - `INSUFFICIENT_FUNDS` if change cannot be provided.
  - `CLOSED` if drawer cash matches the change due exactly.
  - `OPEN` when change is successfully returned.

---

## Files

- `index.html` — The main HTML file containing the UI.
- `script.js` — JavaScript logic for processing purchase and change calculation.

---

## How to Use

1. Open `index.html` in a modern web browser.
2. Enter the amount of cash given by the customer.
3. Click the **Purchase** button.
4. The change due or relevant status message will display below.

---

## Variables to Modify for Testing

- `price` — Set the purchase price in `script.js` for different scenarios.
- `cid` — Cash in drawer array in `script.js`. Modify amounts and denominations to test various drawer states.

---

## Currency Units

The app uses the following denominations for change calculation:

| Unit         | Value  |
| ------------ | ------ |
| PENNY        | $0.01  |
| NICKEL       | $0.05  |
| DIME         | $0.10  |
| QUARTER      | $0.25  |
| ONE          | $1.00  |
| FIVE         | $5.00  |
| TEN          | $10.00 |
| TWENTY       | $20.00 |
| ONE HUNDRED  | $100.00|

---

## Example Scenarios

- **Insufficient cash**: Customer provides less money than price → alert shown.
- **Exact cash**: Cash equals price → message: *No change due*.
- **Change due with open drawer**: Change returned in coins and bills.
- **Change due with closed drawer**: Drawer cash equals change due → status `CLOSED`.
- **Insufficient funds in drawer**: Drawer can’t provide exact change → status `INSUFFICIENT_FUNDS`.

---

## Dependencies

- No external libraries or frameworks are required.
- Tested on modern browsers supporting ES6 JavaScript.

---

## License

This project is open-source and free to use and modify.

---

## Author

Created by Jordan Leturgez

---
