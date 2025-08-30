# Decision Table – Login outcome

| Case | Username present | Password present | Creds valid | Expected outcome      |
|-----:|:----------------:|:----------------:|:-----------:|-----------------------|
| 1    | Y                | Y                | Y           | Login → dashboard     |
| 2    | Y                | Y                | N           | Invalid credentials   |
| 3    | Y                | N                | –           | “Required” password   |
| 4    | N                | Y                | –           | “Required” username   |
| 5    | N                | N                | –           | Require both fields   |

> Technique: Decision table (*tabla de decisión*). Complements EP/BVA.

# State Transition (Login)

[LoggedOut] --(valid creds)--> [LoggedIn]
[LoggedOut] --(invalid/empty)--> [LoggedOut]

[LoggedIn] --(logout)--> [LoggedOut]
# Expected after logout:
[LoggedOut] --(browser Back)--> [LoggedOut]

# Actual (DEF-014):
[LoggedOut] --(browser Back)--> [LoggedIn]   <-- BUG


## Coverage map

| Case | Inputs (Username/Password/Creds valid) | Expected outcome            | Covered by TCs |
|-----:|----------------------------------------|-----------------------------|----------------|
| 1    | Y / Y / Y                              | Login → dashboard           | TC-001, TC-012 |
| 2    | Y / Y / N                              | Invalid credentials         | TC-004, TC-005, TC-013 |
| 3    | Y / N / –                              | “Required” password         | TC-003 |
| 4    | N / Y / –                              | “Required” username         | TC-002 |
| 5    | N / N / –                              | Require both fields         | TC-008 |

**Related defect:** [DEF-014 – Logout allows back navigation](./defects/DEF-014_logout_back.md)

