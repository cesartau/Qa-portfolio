# DEF-014 – Logout allows back navigation
Severity: Medium • Priority: High  
Environment: Windows 11, Firefox

**Steps to Reproduce**
1) Login as Admin / admin123
2) Open user menu → Logout
3) Press browser **Back**

**Expected**  
Remain on login; dashboard not accessible.

**Actual**  
Back shows the user menu / dashboard is accessible.

**Evidence**  
![](../evidence/TC-014_state-trantittion_Defect_2025-08-25.png)
![](../evidence/TC-014_state-trantittion_Defect_2_2025-08-25.png)

**Notes**  
Likely missing cache-control/no-store on authenticated pages.
