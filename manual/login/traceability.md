# Login – Quick Traceability (no charts)

**Purpose:** One-screen map from requirements → test cases → result.  
**Env:** Windows 11 • Firefox  **Creds:** Admin / admin123

Legend: ✅ PASS 🟠 Defect logged 📝 Clarification/UX

| # | Requirement (what should happen)                                   | Test case(s)        | Result |
|---|--------------------------------------------------------------------|---------------------|:------:|
| 1 | Valid login opens the dashboard                                    | [TC-001](./test-cases.md), [TC-012](./test-cases.md) | ✅ |
| 2 | Username required when blank                                       | [TC-002](./test-cases.md)                           | ✅ |
| 3 | Password required when blank                                       | [TC-003](./test-cases.md)                           | ✅ |
| 4 | Wrong credentials show “Invalid credentials”                       | [TC-004](./test-cases.md), [TC-013](./test-cases.md) | ✅ |
| 5 | Username case policy is handled (defined/insensitive)              | [TC-005](./test-cases.md)                           | ✅ |
| 6 | After **Logout**, pressing browser **Back** does **not** reopen app | [TC-014](./test-cases.md)                           | 🟠 See [DEF-014](./defects/DEF-014_logout_back.md) |
| 7 | Password is masked; toggle works *if present*                      | [TC-015](./test-cases.md)                           | 📝 See [CLAR-002](./defects/CLAR-002_password_toggle.md) |

## Links
- Test cases: [./test-cases.md](./test-cases.md)
- Defect (logout + back): [./defects/DEF-014_logout_back.md](./defects/DEF-014_logout_back.md)
- Clarification (password toggle): [./defects/CLAR-002_password_toggle.md](./defects/CLAR-002_password_toggle.md)
- Evidence (screens): [./evidence/](./evidence/)
