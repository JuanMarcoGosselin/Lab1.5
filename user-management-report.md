## 📄 `docs/user-management-report.md`

```markdown
# User Management Report - Lab 1.5

**Student:** [Juan Marco Gosselin Gamboa] 
**Date:** [29 sep 2025]  
**Course:** Operating Systems  

---

## Users Created
| User     | Groups                    | Home Directory  | Shell      | Purpose              |
|----------|---------------------------|-----------------|------------|----------------------|
| alice    | developers, administrators, sudo | /home/alice     | /bin/bash | Lead Developer       |
| bob      | developers                | /home/bob       | /bin/bash | Junior Developer     |
| charlie  | testers                   | /home/charlie   | /bin/bash | QA Tester            |
| temp_user | (default)                | /home/temp_user | /bin/bash | Temporary account (expires 2024-12-31) |
| service_account | (system)           | /               | /usr/sbin/nologin | Service account for background tasks |

---

## Groups Created
- **developers**: Alice (Lead), Bob (Junior)  
- **testers**: Charlie (QA)  
- **administrators**: Alice (admin role)  

Verification command:  
```bash
cat /etc/group | grep -E "(developers|testers|administrators)"
