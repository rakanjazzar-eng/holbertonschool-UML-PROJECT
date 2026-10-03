# Design Justification

## Main Design Decisions

We designed the system around the Order because it is the main part of the food delivery process.

The Platform coordinates the interactions between the User, Order, and Restaurant.

We only included the components required by the scenario and avoided unnecessary features such as payment and delivery routing.

## Responsibilities

- User represents the customer and receives notifications.
- Restaurant provides menu items and confirms orders.
- MenuItem represents an item offered by a restaurant.
- Order contains selected items and manages its status.
- OrderStatus represents the order states: CREATED, CONFIRMED, PREPARED, and DELIVERED.
- Platform coordinates the main operations of the system.

## Relationships and Multiplicities

A User can place multiple Orders, but each Order belongs to one User.

A Restaurant can receive multiple Orders, but each Order is associated with one Restaurant.

A Restaurant offers multiple MenuItems.

An Order contains multiple MenuItems.

Each Order has one current OrderStatus.

## Alternatives and Trade-offs

We considered adding payment, delivery routing, and other features, but they were not required by the scenario.

Keeping the design simple makes the system easier to understand and avoids unnecessary complexity.

