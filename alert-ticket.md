# Alert Ticket A-2703

| Ticket ID | Alert Message | Severity | Details | Ticket Status |
|---|---|---|---|---|
| A-2703 | SERVER-MAIL Phishing attempt possible download of malware | Medium | The user may have opened a malicious email and opened attachments or clicked links | **Escalated** |

## Additional Information

Known malicious file hash: `54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b`

```
Email:
From: Def Communications <76tguyhh6tgftrt7tg.su>  <114.114.114.114>
Sent: Wednesday, July 20, 2022 09:30:14 AM
To: <hr@inergy.com> <176.157.125.93>
Subject: Re: Infrastructure Egnieer role

Dear HR at Ingergy,

I am writing for to express my interest in the engineer role posted from the website.

There is attached my resume and cover letter. For privacy, the file is password
protected. Use the password paradise10789 to open.

Thank you,

Clyde West

Attachment: filename="bfsvc.exe"
```

## Ticket Comments

The alert was triggered after an employee downloaded and opened an attachment from a phishing email disguised as a job application. Three findings support escalation: first, a sender mismatch, the display name "Def Communications" and the `.su` sending domain don't match the email's signature, "Clyde West," a classic impersonation pattern. Second, the message body contains grammatical errors ("I am writing for to express," "Egnieer" in the subject line) inconsistent with professional correspondence. Third, and most importantly, the attachment `bfsvc.exe` is password-protected, an evasion tactic to bypass automated scanning, and its SHA256 hash was independently confirmed malicious in a prior investigation, matching the Flagpro malware family associated with the BlackTech threat actor. Given the confirmed-malicious attachment and the Medium alert severity, this ticket is being escalated to a Level 2 SOC analyst for further action, including containment of the affected endpoint and a check for lateral movement.
