PROJECT REPORT

-Problem definition:
Build a simple command-line Python tool that takes an order total and a discount percentage, then shows the discount amount and final payable amount for online sales. It helps shoppers and small sellers quickly verify savings and final price.

-Requirement analysis:

Functional: Read order amount and discount percentage (0–100), validate that both are non‑negative and percentage ≤ 100, compute discount and final price, and display all values clearly.

Non‑functional: Use clear names and comments, handle invalid and non‑numeric inputs gracefully, and keep the code beginner‑friendly for standard Python 3.

-Top‑down design / modularization:

1.	Read inputs.

2.	Validate inputs.

3.	Calculate discount amount and final price.

Display results.
Use functions: get_inputs(), calculate_discount(amount, discount_percent), print_summary(amount, discount_percent, discount_amount, final_price), with main() coordinating the flow.

-Algorithm development:

Step 1: Start.
Step 2: Input: amount, discount_percent.

Step 3: Process:

discount_amount = amount * discount_percent / 100

final_price = amount - discount_amount

Step 4: Output: discount_amount, final_price.
Step 5: Validation: show an error and stop if amount < 0 or discount_percent is outside 0–100.
Step 6: Stop

-Testing and refinement:

Tests:

amount = 1000, discount = 0 → discount 0, final 1000.

amount = 2500, discount = 20 → discount 500, final 2000.

amount = 999.99, discount = 100 → discount 999.99, final 0.

Negative or out‑of‑range values and non‑numeric inputs should trigger error messages.

Future improvements: support multiple items, automatic discount tiers, coupon codes, and flat discounts.

