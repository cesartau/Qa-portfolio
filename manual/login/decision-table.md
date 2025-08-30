# Decision Table – Login outcome

| Case | Username present | Password present | Creds valid | Expected outcome      |
|-----:|:----------------:|:----------------:|:-----------:|-----------------------|
| 1    | Y                | Y                | Y           | Login → dashboard     |
| 2    | Y                | Y                | N           | Invalid credentials   |
| 3    | Y                | N                | –           | “Required” password   |
| 4    | N                | Y                | –           | “Required” username   |
| 5    | N                | N                | –           | Require both fields   |

> Technique: Decision table (*tabla de decisión*). Complements EP/BVA.
