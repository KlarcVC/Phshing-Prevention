# Phshing-Prevention

What is the Sender Policy Framework (SPF)? 

- Sender Policy Framework (SPF) is used to authenticate the sender of an email. With an SPF record in place, Internet Service Providers can verify that a mail server is authorized to send email for a specific domain. An SPF record is a DNS TXT record containing a list of the IP addresses that are allowed to send email on behalf of your domain.

What is DKIM?

- DKIM stands for DomainKeys Identified Mail and is used for the authentication of an email that’s being sent.
- DKIM protects message integrity. The content of the email can be verified that it hasn’t been changed while being sent.

What is DMARC?

- DMARC, (Domain-based  Message Authentication Reporting, & Conformance) an open source standard, uses a concept called alignment to tie the result of two other open source standards, SPF (a published list of servers that are authorized to send email on behalf of a domain) and DKIM (a tamper-evident domain seal associated with a piece of email), to the content of an email. If not already deployed, putting a DMARC record into place for your domain will give you feedback that will allow you to troubleshoot your SPF and DKIM configurations if needed.

What is S/MIME? 

- S/MIME (Secure/Multipurpose internet Mail Extensions) is a widely accepted protocol for sending digitally signed and encrypted messages.
- As you can tell from the definition above, the 2 main ingredients for S/MIME are:

Digital Signatures
Encryption
Using Public Key Cryptography, S/MIME guarantees data integrity and nonrepudiation. 

If Bob wishes to use S/MIME, then he'll need a digital certificate. This digital certificate will contain his public key. 
With this digital certificate, Bob can "sign" the email message with his private key. 
Mary can then decrypt Bob's message with Bob's public key. 
Mary will do the same (send her certificate to Bob) when she replies to his email, and Bob complete the same process on his end.
Both will now have each other's certificates for future correspondence. 

![image](https://github.com/user-attachments/assets/a7439189-2cc1-4faa-8b8f-07fa41b9a145)

https://attack.mitre.org/


