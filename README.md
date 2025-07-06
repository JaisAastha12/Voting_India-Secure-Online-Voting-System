# Voting_India-Secure Online Voting System
*Voting India* is a secure and transparent *online voting platform* designed to simulate elections in India, supporting *Lok Sabha, **Vidhan Sabha, and **Local Elections*. It ensures voter privacy, authenticates users with Aadhaar validation, and provides real-time encrypted voting and result display.
---

## 🔐 Key Features

- *Two-Step Login System*
  - Aadhaar-based identity verification
  - Election type & state selection with captcha and second-stage validation

- *Secure Voting*
  - Dynamically generated secret key per user (not stored in DB)
  - Encrypted vote submission to maintain voter anonymity

- *Double Voting Prevention*
  - Checks if the user has already voted
  - Displays “You have already voted” message with animation

- *Real-time Result Display*
  - Vote counts per party
  - Graphical charts (Pie/Bar) with party symbols
  - Result visibility controlled by admin-set timer (date & time-based)

- *Voting Timer*
  - 5-minute countdown to cast vote
  - Auto redirect to homepage after timeout

- *Navigation Protection*
  - Back and refresh button handling to prevent vote manipulation

---

## 🛠 Tech Stack

- *Frontend:* HTML, CSS, JavaScript
- *Backend:* PHP
- *Database:* MySQL
- *Charts:* Chart.js / Google Charts (for results)

---

## 📁 Folder Structure

```plaintext
VotingIndia/
├── index.php
├── login.php
├── voting_login.php
├── vote.php
├── dashboard.php
├── results.php
├── css/
│   └── styles.css
├── js/
│   └── timer.js
├── admin/
│   ├── admin_dashboard.php
│   ├── set_timer.php
│   └── view_results.php
├── sql/
│   └── database.sql
└── README.md
