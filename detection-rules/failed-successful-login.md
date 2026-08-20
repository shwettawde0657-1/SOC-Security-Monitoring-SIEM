# Failed Login Followed by Successful Login

## Objective

Detect authentication activity where failed login attempts are followed by a successful login.

## Detection Concept

A sequence such as:

```text
Failed Login
      ↓
Failed Login
      ↓
Successful Login
