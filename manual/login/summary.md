# Test Summary – Login

**Scope:** OrangeHRM Login  
**Out of scope:** API, non-login modules (PIM, Leave, etc.)  
**Environment:** Windows 11, Firefox  
**Credentials:** Admin / admin123

## Metrics
- Totals: Pass=<3>, Fail=<12>, Clarifications=<1>
- Defects logged: 1 (medium): DEF-014 (Back nav after logout)
- Clarifications: 1 (UX): CLAR-002 (show/hide password toggle not present)

## Risks / Notes
- Back navigation exposes dashboard after logout (security/UX).
- Case-insensitive username accepted (documented as observation in TC-005).

## Exit criteria
- All critical login paths pass; no blocker defects remain.
