# Block 18 Workshop

## Unit Tests

### 1. Function called "multiplication" that returns the product of two input numbers

- Expect multiplication(2, 3) to be **6**
- Expect multiplication(-1, 4) to be **-4**
- Expect multiplication('c', 7) to be **NaN**
- Expect multiplication(9) to be **NaN**
- Expect multiplication() to be **NaN**

### 2. Function called "concatOdds" that takes two arrays of ints as args and returns single array that only contains odd numbers, in ascending order

- Expect concatOdds([4, 3, 2], [8, 5, 1]) to be **[1, 3, 5]**
- Expect concatOdds([-5, 1, 3, 6], [1, 1, 2, 9]) to be **[-5, 1, 3, 9]**
- Expect concatOdds([1, 2, true], ['hello', 4, 5]) to be **[1, 5]**
- Expect concatOdds([1, 2, 3]) to be an **error**

## Functional Tests

### 1. A shopping cart checkout feature that allows a user to check out as a guest (without an account), or as a logged-in user

- When a user clicks checkout as a logged-in user...
  - they should be alerted if the cart is empty
  - they should be shown the total cost of their items
  - they should be asked about their method of payment
  - they should be asked about shipping and billing information
- When a user clicks checkout as a guest...
  - they should be asked if they would like to create an account
    - If yes, they should be prompted to enter an email address and password
      - An error should be thrown if they enter an invalid email address
      - An error should be thrown if the password does not meet the specified requirements
      - A success screen should pop up if they successfully created an account
    - If no, they should continue checking out as a guest
  - they should be asked if they would like to log in
    - An error should be thrown if they enter an invalid email or password
    - An error should be thrown if the fields are left empty
    - A success screen should pop up if they successfully logged in to their account
