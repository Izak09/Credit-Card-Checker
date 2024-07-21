Credit Card Checker
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
This project is a simple JavaScript program designed to validate credit card numbers using the Luhn algorithm. It identifies both valid and invalid card numbers and determines the credit card companies associated with the invalid cards.

The project consists of:

Data Arrays: These arrays represent different batches of credit card numbers categorized into valid, invalid, and mystery cards.
Validation Functions:
- validateCred(cardNumber): Validates if a given card number is valid using the Luhn algorithm.
- findInvalidCards(cards): Filters out invalid card numbers from a batch of card numbers.
- idInvalidCardCompanies(invalidCards): Identifies which credit card companies issued the invalid cards.
- Data Arrays
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
The project includes predefined arrays of card numbers:

1. Valid Cards:

valid1: [4, 5, 3, 9, 6, 7, 7, 9, 0, 8, 0, 1, 6, 8, 0, 8]

valid2: [5, 5, 3, 5, 7, 6, 6, 7, 6, 8, 7, 5, 1, 4, 3, 9]

valid3: [3, 7, 1, 6, 1, 2, 0, 1, 9, 9, 8, 5, 2, 3, 6]

valid4: [6, 0, 1, 1, 1, 4, 4, 3, 4, 0, 6, 8, 2, 9, 0, 5]

valid5: [4, 5, 3, 9, 4, 0, 4, 9, 6, 7, 8, 6, 9, 6, 6, 6]


2. Invalid Cards:


invalid1: [4, 5, 3, 2, 7, 7, 8, 7, 7, 1, 0, 9, 1, 7, 9, 5]

invalid2: [5, 7, 9, 5, 5, 9, 3, 3, 9, 2, 1, 3, 4, 6, 4, 3]

invalid3: [3, 7, 5, 7, 9, 6, 0, 8, 4, 4, 5, 9, 9, 1, 4]

invalid4: [6, 0, 1, 1, 1, 2, 7, 9, 6, 1, 7, 7, 7, 9, 3, 5]

invalid5: [5, 3, 8, 2, 0, 1, 9, 7, 7, 2, 8, 8, 3, 8, 5, 4]


3. Mystery Cards:


mystery1: [3, 4, 4, 8, 0, 1, 9, 6, 8, 3, 0, 5, 4, 1, 4]

mystery2: [5, 4, 6, 6, 1, 0, 0, 8, 6, 1, 6, 2, 0, 2, 3, 9]

mystery3: [6, 0, 1, 1, 3, 7, 7, 0, 2, 0, 9, 6, 2, 6, 5, 6, 2, 0, 3]

mystery4: [4, 9, 2, 9, 8, 7, 7, 1, 6, 9, 2, 1, 7, 0, 9, 3]

mystery5: [4, 9, 1, 3, 5, 4, 0, 4, 6, 3, 0, 7, 2, 5, 2, 3]

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
FUNCTIONS:

- validateCred(cardNumber)
- Validates a credit card number using the Luhn algorithm:
- Reverses the card number.
- Doubles every second digit from the right.
- Subtracts 9 from any doubled number greater than 9.
- Sums all the digits.
- Returns true if the total sum is divisible by 10, otherwise false.
- findInvalidCards(cards)
- Filters out invalid card numbers from a given array of card numbers using validateCred.
- idInvalidCardCompanies(invalidCards)
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Identifies which credit card companies issued the invalid cards:

3: American Express (Amex)

4: Visa

5: Mastercard

6: Discover

Returns an array of unique company names.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
To conclude, The Credit Card Checker project serves as an efficient JavaScript tool for validating credit card numbers using the LUHN ALGORITHM.
