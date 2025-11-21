# 🔒 Task 6: Strong Password Evaluation Report

## Objective & Deliverables

**Objective:** Understand what makes a password strong and test it against various online password strength checkers to evaluate its security and resistance to common attacks.

**Deliverable:** A report detailing password strength testing results, analysis of attack vectors, best practice tips, and answers to key cybersecurity interview questions.

---

## I. Password Strength Testing Results

The following table documents the testing of various password types, demonstrating the impact of length and complexity (entropy) on security.

| Password Type | Example Password | Length | Complexity (Char Set) | Estimated Crack Time | Key Learning Point |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Very Weak** | `password` | 8 | Lowercase only | **< 1 Second** | Simple dictionary words are instantly compromised. |
| **Weak** | `P@ssw0rd` | 8 | Mixed, Num, Symbol | **~ 2 Hours** | High complexity with short length is still easily brute-forced. |
| **Medium** | `Zebra%9!Book=3` | 13 | Mixed, Num, Symbol | **~ 20 Years** | Moderate length with full complexity offers better security, but could be cracked eventually. |
| **Strong** | `Tr0ubl3P!zzaFr1dge` | 18 | Mixed, Num, Symbol | **~ 8 Quintillion Years** | Long passphrases with complexity are the strongest due to massive keyspace. |
| **Very Strong** | `L0ngR@nd0mP#r@s3` | 16 | Mixed, Num, Symbol | **~ 9 Billion Years** | Length combined with randomness provides extreme resistance to cracking. |

---

## II. Analysis and Best Practices

### A. Summary of Security Affects (Brute Force vs. Dictionary)

1.  **Brute Force Attack:** This attack attempts every single combination of characters until the password is found.  A strong password defeats this by maximizing the **keyspace**. For every character added, the number of combinations grows **exponentially** ($C^L$). As seen in the table, moving from an 8-character password to an 18-character password increases the crack time from hours to quintillions of years, rendering the attack impractical.

2.  **Dictionary Attack:** This attack uses a pre-compiled list of common passwords, phrases, and personal information. Strong passwords defeat this by simply **not being included** in the dictionary list. Passwords like `password` are instantly found, while unique, non-dictionary passphrases like `Tr0ubl3P!zzaFr1dge` are highly resistant.

### B. Password Best Practice Tips

Based on the evaluation, these tips maximize password security:

1.  **Prioritize Length (14+ Chars):** Length has the most significant impact on security. Use **passphrases** (unrelated words strung together) for easier recall and greater length.
2.  **Use Unique Passwords:** Never reuse the same password across multiple sites to prevent widespread compromise after a single data breach.
3.  **Use a Password Manager:** This is crucial for **generating** and **securely storing** the unique, long, and complex passwords required for all services.
4.  **Enable Multi-Factor Authentication (MFA/2FA):** Use a secondary verification method (like an authenticator app or security key) to protect accounts even if the password is stolen.
5.  **Avoid Personal and Dictionary Information:** Never use common dictionary words, names, or simple sequential patterns, as these are targeted by Dictionary Attacks.
