# Alex

Inbound AI phone receptionist for a small agency that serves more than one client from one deployment.

## Problem

Missed calls lose jobs. A single shared number does not tell you which business was dialed, and a receptionist that only works for one tenant does not fit an agency.

## What I built

- Inbound call handling on Twilio that captures caller intent
- Routing by the number that was dialed, so one cloud app serves many clients
- Dashboard of conversations
- Agency API and a Windows agency console for managing tenants
- SQLite for the app database, with no native build step on Windows

## Stack

Next.js, TypeScript, Twilio, Node.js, SQLite, Electron agency console.

## Status

Private phase-1 product. This page does not include phone numbers, tokens, or webhook URLs.
