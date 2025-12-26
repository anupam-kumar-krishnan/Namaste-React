# _Monolith and Microservice Architechture_

Monolithic architecture is a single deployable application where all modules are tightly coupled. Microservices architecture breaks the application into small independent services that communicate over APIs, allowing independent scaling and deployment.

### Why Microservices?

Microservices improve scalability, fault isolation, and team productivity but increase operational complexity and require DevOps maturity.

<img width="1489" height="585" alt="image" src="https://github.com/user-attachments/assets/c8dfcc01-5933-4499-aa7e-e2d49063ea6e" />

### Separation of Concerns (SoC)

Separation of Concerns means:
> Divide a system into distinct sections, where each section handles a specific concern.

> Separation of Concerns is a design principle that splits an application into independent sections, each responsible for a specific functionality.

**A concern is anything the program cares about:**

- UI
- Business logic
- Data fetching
- State management
- Styling
- Validation

### 🔍 How SoC is different from SRP

| Principle  |	Scope |
| ---------  | ------ |
| SRP |	One class / function |
| SoC	| Entire application / architecture |

👉 SRP is a part of SoC

### Benefits of SoC

🚀 Scalability<br>
🛠 Maintainability<br>
🧪 Easier testing<br>
♻️ Reusability<br>
👥 Team collaboration<br>

<hr/>

### Single Responsibility Principle (SRP)

The Single Responsibility Principle states:

> A class or module should have only one reason to change.

In simple terms, one class = one responsibility.

### 🧠 Why SRP is important

- ✅ Easier to maintain
- ✅ Easier to test
- ✅ Better readability
- ✅ Fewer bugs when requirements change

### 🔍 What does “responsibility” mean?

A responsibility is a single job or purpose.
If a class does more than one job, changes in one area can break another.

### When to Choose What? 

| Choose Monolith when: | Choose Microservices when: |
| ---- | ---- |
| Small team | High traffic |
| MVP or startup | Large teams |
| Simple business logic | Independent scaling needed |
| Faster time to market | Complex domain logic |


