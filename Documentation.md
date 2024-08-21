# Incident Response Documentation

## Executive Summary

On December 28, 2023, at 7:20 p.m. PT, our organization experienced a security incident where an unauthorized individual gained access to customer personal identifiable information (PII) and financial data. Approximately 50,000 customer records were compromised. The financial impact of the incident is estimated to be $100,000, including direct costs and potential loss of revenue. A thorough investigation has been conducted, and the incident is now closed.

## Incident Timeline

### December 22, 2023
- **3:13 p.m. PT:** An employee received an email from an external address claiming that customer data had been stolen. The sender requested $25,000 in cryptocurrency to avoid releasing the data. The employee assumed the email was spam and deleted it.

### December 28, 2023
- **7:20 p.m. PT:** The same employee received a follow-up email from the same sender. This time, the email included a sample of the stolen customer data and increased the ransom demand to $50,000.
- **7:45 p.m. PT:** The employee notified the security team, who immediately began investigating the incident.

### December 28 - 31, 2023
- The security team conducted a detailed investigation to determine how the data was stolen and the extent of the theft.

## Investigation Details

### Root Cause Analysis
The security team identified the root cause as a vulnerability in the e-commerce web application. Specifically, a forced browsing attack was performed by manipulating the order number in the URL string of the purchase confirmation page. This allowed the attacker to access customer transaction data from thousands of purchase confirmation pages.

### Evidence Collection
- The security team collected and analyzed web application access logs, confirming the attacker's method of accessing sequential customer orders.

## Response and Remediation

### Public Disclosure
- The organization worked with the public relations department to disclose the breach to affected customers.
- Free identity protection services were offered to all impacted customers.

### Technical Remediation
- After analyzing the web server logs, the vulnerability was confirmed and addressed.
- A review of the web application’s access controls and security protocols was initiated.

## Lessons Learned

### Key Takeaways
- The incident highlighted the need for better spam filter settings and employee training on identifying potential threats.
- The importance of promptly reporting suspicious activities was reinforced.

## Recommendations

### Short-Term Actions
- **Routine Vulnerability Scans:** Implement regular scans to identify potential vulnerabilities in web applications.
- **Penetration Testing:** Conduct periodic penetration testing to simulate attacks and uncover weaknesses.

### Long-Term Strategies
- **Access Control Enhancements:**
  - Implement allow listing for URLs to limit access to a specific set of URLs.
  - Ensure that only authenticated users can access sensitive content.
- **Employee Awareness Training:**
  - Provide training to help employees recognize phishing and other social engineering tactics.

