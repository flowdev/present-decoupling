# Decoupling and Code
<h2 class="fragment">Decoupling Through the Ages</h2>
<h2 class="fragment">Decoupling: The Only Advancement in Progamming</h2>

---

## Procedural Programming
![Logo](assets/call-graph.png)

---

## Procedural Programming

In the beginning there was chaos:
- ANYTHING was done to save memory |
- Modifiying code at runtime |
- No chance to reason about the code |

---

## Procedural Programming

Then came procedures:
- they give structure to the program |
- they decouple from registers |
- they decouple from state in the calling procedure |
- they can be reused anywhere in the program |
- they can be reuse across projects |
- This is still used a lot. |

---

## Object Orientation
![Logo](assets/class-diagram.jpg)

---

## Object Orientation

- It grew strong together with GUIs |
- Classes encapsulate functionality and state |
- Thus they decouple from other classes |
- OOP works best for purely technical domains |
- Inheritence creates a lot of coupling |

---

## Clean Code
![Logo](assets/clean-code.jpg)

---

## Clean Code

- Favour Composition over Inheritance |
- Separation of Concerns |
- Information Hiding Principle |
- Tell, don´t ask! (High cohesion) |
- Dependency injection |

---

## Clean Code

SOLID principles:
- Single Responsibility Principle |
- Open Closed Principle |
- Liskov Substitution Principle |
- Interface Segregation Principle |
- Dependency Inversion Principle |

Note:
- Open Closed Principle: open for extension, closed for changes
- Interface Segregation Principle: many client-specific interfaces are better than one general-purpose interface
- Dependency Inversion Principle: one should depend upon abstractions, not concretions

---

## Messaging
![Logo](assets/messaging.jpg)

---

## Messaging

- Why don't we use HTTP internaly? |
- Asynchronism prevents time wise coupling: |
  * no timeout handling
- Persistence prevents stability wise coupling: |
  * no retries with exponential backoff
  * that have to be randomised
  * no circuit breaker
- Sender and receiver are decoupled with messaging. |

---

## Functional Programming
![Logo](assets/lambda.png)

---

## Functional Programming

- Functors (higher-order functions) allow composition of decoupled functions |
- Immutable data structures decouple concurrently running functions |
- Pure (side-effect free) functions are decoupled from any context including timing (lazy evaluation) |

---?image=assets/green-pasture.jpg

## What Can Happen If We Optimize for Decoupling?

---

## What Can Happen If We Optimize for Decoupling?

- Decoupling as a natural thing |
- Great match for business logic |
- Easy to understand |
- Natural graphical representation        |
- Parallel to the Barzahlen solution I am working on a spike implementation for the EBICS service. |
