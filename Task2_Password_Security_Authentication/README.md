# Task 2: Password Security & Authentication

## Oasis Infobyte Cyber Security Internship

---

# Objective

The objective of this report is to explain the importance of password security and authentication mechanisms used to protect user accounts and sensitive information. It covers password creation policies, Multi-Factor Authentication (MFA), password hashing, common password attacks, password managers, and security best practices.

---

# Table of Contents

1. Strong Password Policies
2. Multi-Factor Authentication (MFA)
3. Password Hashing
4. Common Password Attacks
5. Password Managers
6. Best Practices
7. Conclusion

---

# 1. Strong Password Policies

Strong passwords are the first line of defense against unauthorized access. Organizations should implement password policies that encourage users to create secure passwords.

### Characteristics of a Strong Password

- Minimum length of 12–16 characters
- Combination of uppercase and lowercase letters
- Includes numbers and special characters
- Avoids dictionary words
- Avoids personal information
- Unique for every account

### Example

Weak Password:

```
password123
```

Strong Password:

```
T9!m#8Lq@52vXp$
```

---

# 2. Multi-Factor Authentication (MFA)

Multi-Factor Authentication adds an extra layer of security by requiring users to verify their identity using multiple authentication methods.

### Types of Authentication Factors

- Something you know (Password or PIN)
- Something you have (Mobile phone or security key)
- Something you are (Fingerprint or Face Recognition)

### Benefits

- Prevents unauthorized account access
- Protects against stolen passwords
- Improves overall account security

---

# 3. Password Hashing

Password hashing converts passwords into irreversible encrypted values before storing them in a database.

Instead of storing:

```
MyPassword123
```

The system stores:

```
5e884898da280471...
```

### Common Hashing Algorithms

- bcrypt
- Argon2
- PBKDF2
- scrypt

### Advantages

- Passwords are never stored in plain text.
- Difficult for attackers to recover original passwords.

---

# 4. Common Password Attacks

## Brute Force Attack

Attempts every possible password until the correct one is found.

### Prevention

- Account lockout
- MFA
- Strong passwords

---

## Dictionary Attack

Uses a list of common passwords and dictionary words.

### Prevention

- Complex passwords
- Password policies

---

## Credential Stuffing

Uses leaked usernames and passwords from previous data breaches.

### Prevention

- Unique passwords
- Password managers
- MFA

---

## Phishing

Tricks users into revealing their passwords through fake websites or emails.

### Prevention

- Verify website URLs
- User awareness
- MFA

---

# 5. Password Managers

Password managers securely store and generate complex passwords.

### Advantages

- Generates strong passwords
- Stores passwords securely
- Reduces password reuse
- Saves time

### Popular Password Managers

- Bitwarden
- 1Password
- KeePass
- Dashlane

---

# 6. Password Security Best Practices

- Use passwords with at least 12 characters.
- Enable Multi-Factor Authentication.
- Never reuse passwords.
- Store passwords using secure hashing algorithms.
- Use a trusted password manager.
- Regularly update passwords after security incidents.
- Never share passwords.
- Avoid writing passwords on paper.
- Monitor accounts for suspicious login attempts.

---

# Conclusion

Password security is essential for protecting digital accounts and sensitive information. Combining strong password policies, secure password hashing, Multi-Factor Authentication, password managers, and user awareness significantly reduces the risk of unauthorized access and cyberattacks.

---

# References

- NIST Digital Identity Guidelines (SP 800-63B)
- OWASP Password Storage Cheat Sheet
- Microsoft Security Best Practices
- Cybersecurity and Infrastructure Security Agency (CISA)
