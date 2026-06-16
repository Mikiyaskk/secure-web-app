# Secure Web Application Project

A Flask web application built to show web security vulnerabilities and their fixes.

## About This Project
While building this login application, I discovered that user input was being passed directly into database queries, which would 
allow an attacker to bypass authentication. 
I researched the issue, identified it as SQL Injection, then found a second vulnerability, XSS in the comments feature. 
Both were documented and fixed.

## Vulnerabilities Demonstrated
- **SQL Injection** — bypassed authentication using malicious input, fixed with parameterized queries
- **XSS (Cross-Site Scripting)** — injected scripts via comments, fixed by removing unsafe rendering
- **Plain Text Passwords** — fixed with bcrypt hashing

## Tech Stack
Python, Flask, SQLite, bcrypt

## How To Run
pip install flask bcrypt
python3 app.py

Then visit http://localhost:5000
