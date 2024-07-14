# Credit Card Validator

The "Credit Card Checker" project is a coding challenge from Codecademy.It project provides a set of JavaScript functions to validate credit card numbers using the Luhn algorithm, identify invalid cards, as well as determine the companies that issued these invalid cards based on their first digit.

## Functions

### 1. `validateCred(arr)`

This function validates a credit card number using the Luhn algorithm. It takes an array of digits (`arr`) representing the credit card number and returns `true` if the number is valid, and `false` otherwise. The original array (`arr`) is not mutated.

### 2. `findInvalidCards(nestedArray)`

This function checks through a nested array of credit card numbers (`nestedArray`) and returns another nested array containing only the invalid card numbers. It utilizes the `validateCred` function to determine the validity of each card number.

### 3. `idInvalidCardCompanies(array)`

This function identifies and returns an array of companies that issued the invalid credit card numbers based on their first digit. It takes a nested array (`array`) of invalid card numbers and maps each company to its corresponding first digit as follows:

- **3**: "Amex (American Express)"
- **4**: "Visa"
- **5**: "Mastercard"
- **6**: "Discover"

If a card number does not start with any of these digits, the function outputs "Company not found".
