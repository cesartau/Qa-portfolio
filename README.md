# OrangeHRM – QA Practice Portfolio (ISTQB FL 4.0)

**Goal:** Demonstrate manual testing using ISTQB techniques (EP, BVA, Decision Table, State Transition).  
**Scope:** Login feature of OrangeHRM (open-source demo).

## Quick view
- **Techniques:** EP/BVA, Decision Table, State Transition (ES: Partición de Equivalencia, Valores Límite, Tabla de Decisión, Transición de Estados)
- **Environment:** Windows 11, Firefox
- **Creds used:** Admin / admin123
- **Results:** Pass: <X> | Fail: <Y> | Defects: <Z>

## Navigate
- **Test Cases:** [`manual/login/test-cases.md`](manual/login/test-cases.md)
- **Decision Table & State Transition:** [`manual/login/decision-table.md`](manual/login/decision-table.md)
- **Defects:** [`manual/login/defects/`](manual/login/defects/)
  - Back nav after logout: [`DEF-014_logout_back.md`](manual/login/defects/DEF-014_logout_back.md)
  - Clarification (not a bug): [`CLAR-002_password_toggle.md`](manual/login/defects/CLAR-002_password_toggle.md)
- **Evidence (screens):** [`manual/login/evidence/`](manual/login/evidence/)
- **Summary report:** [`manual/login/summary.md`](manual/login/summary.md)
- **Traceability matrix**[`Qa-portfolio/manual/login/traceability.md`]
## Folder map

manual/
login/
decision-table.md
summary.md
test-cases.md
defects/
CLAR-002_password_toggle.md
DEF-014_logout_back.md
evidence/
TC-005_username-case_FAIL_2025-08-25.png
TC-014_state-trantition_Defect_2025-08-25.png


## How to reproduce key defect
- Open user menu → Logout → press browser **Back** → dashboard becomes accessible (should not).
