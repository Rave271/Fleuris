# Group 8 - Submission File

> **Instructions:** Every student in this group must fill in their own section below.  
> Do **not** leave any field blank. Replace all placeholder text with real information.  
> This file must be placed inside `student_folder/grp8/grp8_group_info.md` before raising your PR.

---

## Project Details

| Field | Details |
| --- | --- |
| **Group Number** | Group 8 |
| **Project Name** | Fleuris Vault Bank |
| **Reference Used** | Unsafe Banking |
| **Branch Name** | `grp8-FleurisVaultBank` |
| **Deployed URL** | Local demo: `http://127.0.0.1:5001/` |

---

## Student Details

### Student 1

| Field | Details |
| --- | --- |
| **Full Name** | MEHAK GUPTA |
| **Roll Number** | 2310991984 |
| **GitHub Profile** | `https://github.com/MehakGupta1725` |
| **Assigned Vulnerability** | Security Misconfiguration / Missing Security Headers |
| **Contribution** | Led the project documentation and PPT reference material. Prepared the detailed project explanation, security concept write-up, presentation flow, demo explanation notes, and summary of how Fleuris Vault Bank improves the unsafe banking reference project. Also documented the security header improvements such as Content-Security-Policy, X-Frame-Options, X-Content-Type-Options, and Referrer-Policy. |

---

### Student 2

| Field | Details |
| --- | --- |
| **Full Name** | JASHANJOT SINGH |
| **Roll Number** | 2310992023 |
| **GitHub Profile** | `https://github.com/jashanjotahujla` |
| **Assigned Vulnerability** | SQL Injection |
| **Contribution** | Supported the SQL injection prevention section by explaining how unsafe query building can be abused and how the project uses parameterized SQLite queries such as `WHERE username=?` to treat input as data. Also helped with general file organization and final review. |

---

### Student 3

| Field | Details |
| --- | --- |
| **Full Name** | JASHAN YADAV |
| **Roll Number** | 2310992105 |
| **GitHub Profile** | `https://github.com/Jxstiin` |
| **Assigned Vulnerability** | Brute Force Login Attempts |
| **Contribution** | Covered the brute-force protection explanation, including failed login counting, temporary account lockout after repeated failures, and demo steps for showing the lockout behavior. Also helped with small cleanup, formatting, and filler content required for the final submission. |

---

### Student 4

| Field | Details |
| --- | --- |
| **Full Name** | ARYAN GUPTA |
| **Roll Number** | 2310992114 |
| **GitHub Profile** | `https://github.com/abey-aryan` |
| **Assigned Vulnerability** | Cross-Site Request Forgery on Money Transfers |
| **Contribution** | Worked on the secure transfer flow and coding explanation for CSRF protection. Covered how the transfer form includes a hidden session-bound CSRF token and how invalid or missing tokens are rejected before any balance update is performed. |

---

### Student 5

| Field | Details |
| --- | --- |
| **Full Name** | VANSHIKA SARDANA |
| **Roll Number** | 2310992171 |
| **GitHub Profile** | `https://github.com/vanshika280` |
| **Assigned Vulnerability** | Weak Password Storage |
| **Contribution** | Contributed a brief coding and documentation role for password security. Explained the move from plain password handling to hashed password verification using Werkzeug's `generate_password_hash()` and `check_password_hash()`, and documented why password hashes reduce risk if the database is exposed. |

---

### Student 6

| Field | Details |
| --- | --- |
| **Full Name** | RAGHAV VERMA |
| **Roll Number** | 2310992187 |
| **GitHub Profile** | `https://github.com/Rave271` |
| **Assigned Vulnerability** | Broken Access Control |
| **Contribution** | Worked on the core coding contribution for role-based and ownership-based access control. Implemented and explained checks that prevent customers from viewing other customers' statements, restrict admin-only pages, block admin access to customer transfer flow, and log blocked access attempts as `ACCESS_DENIED`. |

---

## Submission Checklist

Before raising your Pull Request, confirm every item below:

- [x] All 6 student blocks above are fully filled in
- [ ] Deployed URL is working and accessible
- [x] Project code is inside `student_folder/grp8/src/`
- [x] Reference documentation is included in the project folder
- [x] Branch name follows format: `grp8-<project-name>`
- [x] PR is targeting the `develop` branch, not `main`
- [x] No `.env` files or secret keys are committed
- [x] No other group's folder has been touched

---

## Project Description

Fleuris Vault Bank is a Flask-based fintech security project built from an unsafe banking reference application. It provides customer login, dashboards, secure money transfer, account statements, admin review screens, and a Security Demo Lab. The project strengthens common banking workflows using OWASP-style protections such as parameterized SQL, password hashing, account lockout, CSRF protection, role-based access control, security headers, and audit logging. It demonstrates how a vulnerable banking app can be converted into a safer web application with visible security evidence.

---

## Security Concepts Implemented

- SQL injection prevention using parameterized SQLite queries.
- Password hashing using Werkzeug password hashing utilities.
- Brute-force protection through failed login tracking and temporary account lockout.
- Broken access control prevention through customer ownership checks and admin-only route restrictions.
- CSRF protection for the money transfer form using a session-bound token.
- Security misconfiguration reduction through Content-Security-Policy, X-Frame-Options, X-Content-Type-Options, and Referrer-Policy headers.
- Security logging and monitoring through `security.log` and the `security_events` database table.

---

> **Reminder:** Only one person from the group raises the Pull Request.  
> The branch must be created from `develop`, never from `main`.  
> Branch name format: `grp8-your-project-name`
