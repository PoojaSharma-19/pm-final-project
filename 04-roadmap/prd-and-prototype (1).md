# Instant Virtual Mastercard & Apple/Google Wallet, Simplified PRD (Your Riverty case)

**Author:** Me · **Status:** Draft · **Target:** High-Fidelity Prototype · **Persona:** Lena- A 32-year-old salaried employee in Cologne on a middling income with no real cushion, who shops mostly on her phone.

## 1. The Big Picture
- **Vision:** Enable customers to start using their Riverty Mastercard instantly, making "Keep it first, pay later" available everywhere from day one.
- **Press release:** Riverty Introduces Instant Virtual Mastercard—Start Shopping in Minutes, Not Days
Berlin, Germany — Say goodbye to waiting for your card to arrive. Riverty is introducing the Instant Virtual Mastercard, allowing approved customers to add their card to Apple Pay or Google Wallet and start shopping immediately. Whether buying online or paying in-store, customers can now enjoy Riverty's signature "Keep it first, pay later" experience from the moment they're approved—wherever Mastercard is accepted.
For shoppers like Lena, who often has to fall back on her debit card because Riverty isn't available in-store, this changes everything. Instead of paying upfront before deciding whether to keep an item, she can make purchases instantly with her Riverty Mastercard and enjoy the flexibility she's come to expect. By removing the wait between approval and first purchase, Riverty transforms from a checkout payment option into an everyday payment companion—making flexible payments faster, simpler, and always within reach.
- **Success metric:** Active Card Usage Rate- 75% of activated cards used for at least one transaction within 30 days. Why: Shows early adoption and validates that customers are replacing debit cards with Riverty Mastercard.
- **Guardrail:** The percentage of customers who successfully complete a purchase using Riverty BNPL at partner merchants should not decrease after the Mastercard launch.

## 2. The Details
### User stories
- As a newly approved Riverty customer, I want my virtual Mastercard to be available immediately so that I can start using it without waiting for a physical card.
- As a customer, I want to add my Riverty Mastercard to Apple Pay or Google Wallet so that I can pay in-store and online immediately.
- As a customer, I want to securely verify my identity before my virtual card is activated so that my account remains protected.
- As a customer, I want to receive confirmation when my virtual card is activated so that I know it is ready to use.
- As a customer, I want my virtual card to be available in real time after approval so that I can make my first purchase straight away.
- As a customer, I want clear instructions for adding my card to my digital wallet so that I can complete the setup without confusion.
- As a customer, I want to receive a notification when my card is successfully added to my wallet so that I know I can start paying immediately.
- As a customer, I want to view my virtual card details and wallet status in the Riverty app so that I can easily manage my card.
- As a customer, I want to receive real-time notifications after every transaction so that I can track my spending and detect any unexpected activity.
- As a customer, I want to temporarily freeze or unfreeze my virtual card so that I can protect my account if my phone is lost or I suspect fraudulent activity.
### Screens to build
- 1. Entry Point – Card Approved
- Purpose: Inform the customer that their Riverty Mastercard is ready and encourage immediate action.
- Screen Name
- Congratulations! Your Riverty Mastercard is Ready
- UI Elements
- - Success message: "You're approved!"
- - Virtual Mastercard preview
- - Buttons:
- - Add to Apple Pay / Google Wallet
- - View Card Details
- - Key benefits:
- - Use instantly
- - Shop online & in-store
- - No need to wait for your physical card
- Primary CTA: Add to Wallet
- 2. Feature Core – Add to Apple Pay / Google Wallet
- Purpose: Allow customers to securely provision their virtual card to their preferred digital wallet.
- Screen Name
- Add Your Card to Your Wallet
- UI Elements
- - Virtual card preview
- - Apple Pay / Google Wallet selection
- - Secure identity verification prompt (if required)
- - Progress indicator
- - "Add to Wallet" button
- - Help link: Need help setting up?
- Primary CTA: Confirm & Add Card
- 3. Success / Confirmation
- Purpose: Confirm successful setup and encourage the customer's first purchase.
- Screen Name
- You're Ready to Pay
- UI Elements
- - Success icon (✓)
- - Message:Your Riverty Mastercard has been added successfully.
- - Wallet confirmation
- - Suggested next action:
- - Start Shopping
- - Find Partner Merchants
- - Small reminder:Keep it first, pay later—wherever Mastercard is accepted.
- Primary CTA: Start Shopping
### Functional requirements
- FR1 – Instant Virtual Card Generation
- FR2 – Apple Pay & Google Wallet Provisioning
- FR3 – Secure Customer Authentication
- FR4 – Real-Time Card Activation
- FR5 – Card Ready Confirmation
- FR6 – Immediate Payment Readiness
- FR7 – Wallet Provisioning Status
- FR8 – Error Handling
### Smart behaviors (Situation → Outcome)
- Smart Behaviors (If → Then)
- - If a customer is successfully approved for a Riverty Mastercard, then the system generates a virtual Mastercard and makes it available within 30 seconds.
- - If the virtual Mastercard is generated successfully, then the system prompts the customer to add it to Apple Pay or Google Wallet.
- - If identity verification is required before wallet provisioning, then the system requests authentication before continuing.
- - If the customer successfully adds the card to Apple Pay or Google Wallet, then the system displays a confirmation message and sends a push notification.
- - If wallet provisioning fails, then the system displays the reason for the failure and provides an option to retry.
- - If the customer makes their first successful purchase using the Riverty Mastercard, then the system sends a real-time transaction notification and encourages continued card usage.
- - If the customer has not added the virtual card to a digital wallet within 24 hours of approval, then the system sends a reminder to complete wallet setup.
- - If the customer has activated the card but has not completed a transaction within 7 days, then the system sends a personalised reminder highlighting the benefits of using the Riverty Mastercard.
### Technical constraints
- No physical card fulfilment
- No automatic wallet provisioning across multiple devices

## 3. The Logistics
### Features out
- Spending Analytics Dashboard
- Multi-Currency Support
- AI-Powered Spending Insights
### Edge cases & safety guard
- Must never store or transmit payment credentials outside Mastercard, Apple Pay, Google Wallet, and Riverty's approved secure infrastructure.
- Safety Guard (Must NEVER Do)
- - Must never issue a virtual Mastercard before customer identity and eligibility are successfully verified.
- - Must never allow transactions using an inactive, blocked, or expired virtual card.
- - Must never expose the full card number, CVV, or sensitive payment credentials in notifications or unsecured screens.
- - Must never create duplicate virtual cards for the same approved application.
- - Must never store or transmit payment credentials outside Mastercard, Apple Pay, Google Wallet, and Riverty's approved secure infrastructure.
### Decision log
- Decision 1: Prioritise Instant Card Access Over Advanced Card Features
- Decision 2: Support Digital Wallets Only
### Evals
- 1. Accuracy
- Target: ≥ 98% of eligible customers successfully generate and add their virtual Riverty Mastercard to Apple Pay or Google Wallet on their first attempt.
- 2. Time-on-Task
- Target: ≤ 2 minutes for customers to complete the journey from card approval to successful wallet provisioning.
- 3. Safety
- Target: 100% of virtual card activations require successful customer authentication, with 0 unauthorized card activations.

## MoSCoW scope
- **Must:** Instant Virtual Card Generation; Apple Pay & Google Wallet Provisioning; Secure Customer Authentication; Card Activation Confirmation; Real-Time Card Availability
- **Should:** Wallet Setup Guide; Push Notification After Wallet Added; In-App Digital Card View; Sending Notifications after successful notification
- **Could:** Automatic Wallet Provisioning; Device Management; Temporary Card Freeze
- **Won't (now):** Spending analytics dashboards; Multi-currency support; AI-Powered Spending Insights

---
**Builder hook:** Build a working prototype based on this PRD. Use the User Story as the core flow, Functional Requirements as build constraints, and prioritize speed and clarity over visual complexity.
