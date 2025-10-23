# Home IMS (Home Inventory Management System)

## Overview
Home IMS is an open-source system for organizing household storage.  
This project is an extension of a previous Home IMS project.
The goal of this system is to provide a fast, low-friction way to catalog containers and their contents, and to quickly find items later.

## Proposed Tech Stack
This is just a first idea, let's not get too excited/upset about these choices.

### Backend
- Modular Monolithic code base, potentially use microservices for certain features.
- Python for API gateway.
- PostgreSQL

### Frontend
- **Web app:** React (Vite or Next.js, PWA-capable)

#### Future Front End
- **Desktop app:** Electron
- **Mobile app:** React Native (probably) 

### Infrastructure
- **Cloud (default):** Azure
- **Self-host (later):** Docker Compose 

## Scope (MVP)
- User authentication (sign up, login, invite to household)  
- Household → Locations → Containers → Items data model  
- Each container has a **QR code** (deep link)  
- Container screen: list contents, add/edit items, attach photos  
- Global search (fuzzy match across items, containers, notes)  
- Offline-first basic caching (mobile)  
- Self-host support via Docker Compose  

## Roadmap (future ideas)

- NFC tags (tap-to-open, write support)  
- ML-assisted item suggestions from photos  
- Barcode lookup for retail items 
- Export for insurance (CSV/PDF with photos)  