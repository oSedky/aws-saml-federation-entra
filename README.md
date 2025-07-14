# 🛡️ Enterprise-Grade SAML Federation to AWS Using Microsoft Entra ID & Conditional Access

This project implements secure single sign-on to the AWS Console using Microsoft Entra ID (formerly Azure AD) as a SAML 2.0 Identity Provider. It includes MFA enforcement, Conditional Access based on geolocation (Canada), and group-based access control using IAM roles.

---

## 🌐 Architecture Overview

- **Microsoft Entra ID** as SAML 2.0 IdP
- **AWS IAM Identity Provider** to process assertions
- **IAM Roles** mapped to group claims
- **Conditional Access** enforcing MFA and IP-based rules
- **Audit logs** in both platforms

![Federation Architecture](Screenshots/Federation%20AWS%20Azure%20Setup.png)

---

## ✅ Business Impact

- Removes long-term IAM credentials
- Centralized access control
- Fully auditable sign-in workflows
- Meets compliance and security standards

---

## 🔐 Conditional Access Policy

| Feature          | Configuration                    |
|------------------|----------------------------------|
| Assigned Group   | AWS-Users                        |
| Targeted App     | AWS Enterprise Application       |
| Grant Controls   | Require MFA + Trusted Location   |
| Named Location   | Canadian IP ranges               |

---

## 🖼 UI Preview

| Screenshot | Description                         |
|------------|-------------------------------------|
| Entra portal | User sees AWS SSO entry in apps   |
| Role-based landing | Different AWS Console roles |
| Blocked logins | Outside-Canada login blocked    |
| Sign-in logs | Full visibility across platforms  |

---

## 📂 Project Structure

📁 Project-01-Federation-AWS-M365
├── saml-federation.html # Full implementation doc
├── LICENSE # MIT License
├── README.md # This file
├── Screenshots\ # 23 screenshots + architecture
└── Metadata\aws-saml-idp.xml # SAML metadata for import

less
Copy
Edit

---

## 📬 Contact

- LinkedIn: [Omar Sedky](https://www.linkedin.com/in/omarsedky)
- GitHub: [@oSedky](https://github.com/oSedky)
- Email: omar@sedky.net