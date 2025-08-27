# CLAR-002 — Password visibility toggle (TC-015)
Status: Open  (aclaración)
Linked TC: TC-015

Observed:
- Password is masked; there is **no** show/hide toggle. TC-015 = PASS.

Question:
- Is a **show/hide password** toggle expected on the Login page?

Impact:
- If “Yes”, we’ll log an enhancement and add tests for the toggle behavior.
- If “No”, TC-015 remains PASS as-is.

Steps to check:
1) Open Login
2) Type in Password field and look for a visibility control
3) Observe masking
