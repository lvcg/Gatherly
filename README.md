# accesscentre — Event Management & Ticketing

accesscentre is a responsive event marketplace and organizer dashboard built from the original QR Code Generator. It demonstrates a connected attendee and organizer journey: event discovery, filtering, demo checkout, unique QR ticket generation, a persistent ticket wallet, event creation, and QR check-in simulation.

## Run locally

Serve the folder instead of opening the HTML file directly (the PWA service worker requires HTTP):

```bash
npx serve .
```

## Demo flow

1. Open an event from **Discover** and select **Get tickets**.
2. Complete the demo checkout. Tickets persist in local browser storage.
3. Open **My tickets** and select a pass to enlarge its unique QR code.
4. Open **Organizer**, launch the scanner, and simulate a guest check-in.
5. Use **Create event** to preview the organizer publishing flow.

## Production architecture path

This dependency-light PWA prototype can evolve into Next.js App Router, PostgreSQL/Prisma transactions, Stripe Payment Intents, signed rotating ticket tokens, Cloudinary uploads, and camera scanning with `BarcodeDetector` or `html5-qrcode`.
