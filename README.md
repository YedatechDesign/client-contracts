# client-contracts
digital contracts with clients

# Client Contracts System

This repository contains the digital contract signing system used by Yeda.

## Files

admin.html  
Admin panel used by the company to create and edit contracts for clients.

proposal.html  
Client page where the client can read the contract, fill required fields and sign it digitally.

## How it works

1. The company opens the admin panel.
2. A contract is created and saved.
3. A link is sent to the client.
4. The client opens the link, fills the required fields and signs the contract.
5. The system generates a signed PDF.
6. The PDF is saved in Google Drive and sent by email.

## Automation

The backend automation is handled by **n8n** workflows which:
- save contract data
- load contracts
- generate signed PDFs
- store them in Google Drive
- send emails to the company and the client
