# Java Inheritance - Newspaper Subscriptions

A Java practical demonstrating **inheritance, abstract classes and method overriding** through a newspaper subscription system with two subscription types.

## How it works

| Class | Role |
|-|-|
| `NewspaperSubscription` | Abstract base class holding the subscriber's name, address and rate, with getters, setters and `toString()` |
| `PhysicalNewspaperSubscription` | Home delivery. Overrides `setSubscriberAddress()` so the address must contain at least one digit (a street number); valid addresses get a rate of R15.00, invalid ones R0 with an error message |
| `OnlineNewspaperSubscription` | Online delivery. Overrides `setSubscriberAddress()` so the address must be an email (contains `@`); valid addresses get a rate of R9.00, invalid ones R0 with an error message |
| `DemoSubscriptions` | Driver program that creates one subscription of each type and prints the name, address and rate |

## Concepts practised

- Abstract classes and inheritance
- Method overriding with `super` calls
- Input validation inside setters
- Polymorphic behaviour from a shared base class

## Running the code

Requires JDK 8+.

```bash
javac *.java
java DemoSubscriptions
```

> Note: the file `PhysicalNewspapaerSubscription.java` should be renamed to `PhysicalNewspaperSubscription.java` (matching its class name) for it to compile.

## Author

**Mohau Mokoena**
