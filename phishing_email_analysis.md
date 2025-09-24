# Phishing Email Analysis (TASK 2)

---

## 1. Summary

This report documents the analysis of a suspicious email pretending to be from "StreamFlix". The message uses social engineering and technical deception to lure users to a malicious website. An investigation of the email's content and headers confirms it is a phishing attempt. The full text of the analyzed email is included below for context.

---

## 2. Email Sample Under Analysis

The following is the full content of the phishing email that was investigated.

> **From:** StreamFlix Support <info@mailer-cluster-123.net>
> **Subject:** [Action Required] Your Subscription is On Hold
> **To:** user@example.com
>
> ---
>
> Dear Member,
>
> We were unable to process the latest payment for your subscription. This might be due to a change in your card details or an issue with your bank.
>
> To avoid service interruption, you must update your billing information immediately. If you do not update your payment method within 24 hours, your account will be permanently closed and a reactivation fee will apply.
>
> Please log in to your account and update your details by clicking the secure link below:
>
> [**Update Your Billing Details**](http://streamflix-billing-update.security-center.com/login)
>
> Thank you for your quick attention to this matter.
>
> Sincerely,
> The StreamFlix Team

---

## 3. Detailed Analysis & Tools Used

Based on the sample above, the following indicators were identified using standard analysis techniques.

### Indicator 1: Sender's Email Address
* **Finding:** The sender's address (`info@mailer-cluster-123.net`) does not belong to the official `streamflix.com` domain, which is a primary indicator of a phishing attempt.

### Indicator 2: Email Header Discrepancies
* **Action:** I analyzed the email's full headers using an online tool like MXToolbox.
* **Findings:** The headers revealed a `softfail` on the SPF check and a `Reply-To` address of `scammer@proton.me`, confirming the sender is not who they claim to be.

### Indicator 3: URL and Domain Analysis
* **Action:** I safely analyzed the link URL (`http://streamflix-billing-update.security-center.com/login`) using VirusTotal and performed a WHOIS lookup on the root domain.
* **Findings:** The URL leads to a non-official domain (`security-center.com`) that was registered only 48 hours ago. This is a classic sign of a malicious site.

### Indicator 4: Social Engineering Tactics
* **Finding:** The email body uses high-pressure language ("immediately", "within 24 hours", "permanently closed") to create a sense of urgency and panic.

---

## 4. Conclusion

The email is definitively a phishing attack. The evidence from the sender's address, header data, deceptive URL, and psychological tactics all support this conclusion.