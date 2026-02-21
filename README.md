# Discount_Calculator

This repository contains a small utility for calculating discounted prices.

Function `apply_discount(price, discount)` (in `dis_cal.py`):

- **Purpose:** Validate inputs and compute the final price after applying a percentage discount.
- **Parameters:** `price` (int or float), `discount` (int or float, percentage 0–100).
- **Validation rules:**
	- Returns the string `'The price should be a number'` if `price` is not numeric.
	- Returns the string `'The discount should be a number'` if `discount` is not numeric.
	- Returns the string `'The price should be greater than 0'` if `price <= 0`.
	- Returns the string `'The discount should be between 0 and 100'` if `discount < 0` or `discount > 100`.
- **Return value:** The final price as a number (price minus percentage discount) when inputs are valid.

Example usage:

```python
from dis_cal import apply_discount

print(apply_discount(100, 20))   # -> 80.0
print(apply_discount('a', 20))   # -> 'The price should be a number'
```

File: `dis_cal.py` implements the function and basic input validation.