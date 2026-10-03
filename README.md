# Food Delivery Platform

## Problem Analysis

### Main Entities

- User
- Restaurant
- MenuItem
- Order
- OrderStatus
- Platform

### Main Relationships

- A User can place multiple Orders.
- Each Order belongs to exactly one User.
- A Restaurant offers multiple MenuItems.
- Each MenuItem belongs to exactly one Restaurant.
- A Restaurant can receive multiple Orders.
- Each Order is associated with exactly one Restaurant.
- An Order contains multiple MenuItems.
- Each Order has exactly one OrderStatus.

### Main Use Cases

1. Place an order
2. Add an item to an order
3. Update order status
