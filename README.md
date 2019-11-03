# Discount Calculator

```json
{
  "customer-1": [
    { "product": "bred", "quantity": 28 },
    { "product": "chocolate", "quantity": 18 },
    { "product": "cake", "quantity": 7 }
  ]
}
```

Discount distribution

| Quantity Range | Discount Rate |
| -------------- | ------------- |
| 0-35           | 0%            |
| 36-50          | 5%            |
| 51-            | 10%           |

Expected allocation

```json
{
  "customer-1": [
    ["bred", "10%", 3],
    ["bred", "5%", 15],
    ["bred", "0%", 10],
    ["chocolate", "0%", 18],
    ["cake", "0%", 7]
  ]
}
```
