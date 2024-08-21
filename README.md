# Incident Response Report

## Executive Summary

On December 28, 2023, a security incident occurred where an unauthorized individual gained access to approximately 50,000 customer records containing personal identifiable information (PII) and financial data. The financial impact is estimated at $100,000. A thorough investigation has been completed, and the incident is now closed.

## Timeline

- **December 22, 2023, 3:13 p.m. PT:** An employee received an extortion email claiming customer data theft, which was dismissed as spam.
- **December 28, 2023, 7:20 p.m. PT:** The employee received a follow-up email with a sample of stolen data and a ransom demand. The security team was notified, and an investigation began.
- **December 28 - 31, 2023:** The security team identified a vulnerability in the e-commerce web application, leading to the theft of customer data.

## Investigation

The investigation revealed a forced browsing attack exploiting a vulnerability in the e-commerce application. By manipulating the order number in the URL, the attacker accessed and exfiltrated customer transaction data.

## Response and Remediation

- The organization disclosed the breach to affected customers and offered free identity protection services.
- The security team confirmed the cause through web server logs, showing a high volume of sequential customer order access.

## Recommendations

To prevent future incidents:

1. Conduct regular vulnerability scans and penetration testing.
2. Implement the following access control mechanisms:
   - Allow listing specific URLs and blocking unauthorized requests.
   - Restrict access to content for authenticated users only.

---

For further details or inquiries, please contact Swaraj Jadhav at swarajj762@gmail.com
