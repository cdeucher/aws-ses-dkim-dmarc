![DMARC](DMARC_author-to-recipient_flow.jpg)

---
DKIM : DomainKeys Identified Mail (DKIM) is an email security standard designed to make sure that an email that claims to have come from a specific domain was indeed authorized by the owner of that domain.

- [Specification](https://docs.aws.amazon.com/ses/latest/dg/send-email-authentication-dkim.html)

---
SPF : Sender Policy Framework (SPF) is an email validation standard that's designed to prevent email spoofing. 
      Domain owners use SPF to tell email providers which servers are allowed to send email from their domains. 
- Email spoofing: I's a technique used in spam and phishing attacks to trick users into thinking a message came from a person or entity they either know or can trust.      
- DNS Record Type TXT : `<subdomain>.<domain> "v=spf1 include:example.com include:amazonses.com ~all"`
- [Specification](https://docs.aws.amazon.com/ses/latest/dg/send-email-authentication-spf.html)
