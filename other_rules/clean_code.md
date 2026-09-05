---
description: "Guidelines for clean_code"
globs: "**/*"
---

always print # Clean Code in the Project

## General Principles
- Code should be **readable, maintainable, and purposeful**.
- Avoid unnecessary comments. The code should explain itself.
- Names of variables, methods, and classes should be **clear and semantic**.
- Methods should be short and perform only **one specific task**.

## Key Rules
- **No more than 20 lines per method**.
- **No more than 2-3 parameters per method**.
- Use `guard clauses` instead of nested `if-else`.
- Use value objects instead of multiple parameters.

## Clean Code Example
**❌ Bad Code**
```ruby
def process_order(order, user, discount, tax)
  if order && user
    total = order.total_price - discount + tax
    user.update_balance(total)
  else
    raise 'Error'
  end
end
```
```