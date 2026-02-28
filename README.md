X: https://x.com/PoPCheckIn

Project: **Proof-of-Presence (Solana Web3 App)**
A blockchain-based Web3 application built on Solana that verifies and records a user's physical presence at events, seminars, or meetups using GPS location, Bluetooth, and NFC, with on-chain proof stored immutably.

**Core Idea**
When a user attends an event:
App verifies geolocation
Confirms proximity using Bluetooth beacon / NFC tag
Wallet signs a transaction
A Proof NFT or on-chain record is minted on Solana
User gets verifiable proof of attendance forever

**Frontend (React)**
Wallet connection (Phantom / Backpack)
Location access (Browser Geolocation API)
Bluetooth (Web Bluetooth API)
NFC (Web NFC API – mobile Chrome)
Event QR fallback option
Transaction signing
NFT display dashboard

**Backend (Node.js)**
Event creation APIs
Event validation logic
Proximity verification logic
Rate limiting & anti-spam protection
Solana transaction building
Optional metadata storage (IPFS/Arweave)

**Solana Program (On-chain Logic)**
You should create:

**Accounts**
Event PDA
Attendance PDA
Verifier PDA
Optional: NFT Mint account

**Instructions**
create_event
verify_presence
mint_proof_nft
close_event
