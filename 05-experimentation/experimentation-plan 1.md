# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Based on qualitative interviews and quantitative evidence showing Riverty's 6% brand preference and that 14% of German BNPL users lose track of outstanding payments, we believe that enabling "Keep it first, pay later" everywhere for Lena—a 32-year-old salaried employee in Cologne with limited financial cushion—will increase everyday Riverty Mastercard usage and strengthen customer loyalty, as measured by an Active Card Usage Rate of at least 75% within 30 days of activation. We will protect the on-time repayment rate (≥98%) and make a go/no-go decision after a 3-month Friends & Family pilot.
- **From M3, your primary success metric & guardrail metric:** Active Card Usage Rate- 75% of activated cards used for at least one transaction within 30 days. Why: Shows early adoption and validates that customers are replacing debit cards with Riverty Mastercard.
The percentage of customers who successfully complete a purchase using Riverty BNPL at partner merchants should not decrease after the Mastercard launch.
- **From M4, the feature you scoped in your PRD this is what you're testing:** Instant Virtual Mastercard & Mobile Wallet- Provides immediate access to the card through Apple Pay or Google Pay after approval, encouraging faster activation and everyday usage without waiting for a physical card.

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** Instant Virtual Mastercard & Mobile Wallet- Provides immediate access to the card through Apple Pay or Google Pay after approval, encouraging faster activation and everyday usage without waiting for a physical card.
- **Persona pull your M2 persona:** Lena- A 32-year-old salaried employee in Cologne on a middling income with no real cushion, who shops mostly on her phone.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** Users can "keep it first, pay later" anywhere, in stores and beyond partner merchants, with one place to see what's due and settle on time. Riverty gets a direct, everyday relationship with its users instead of being just a checkout option. Why launch now:
Regulation: launching now gets an exemption from the CCD2 rules. Klarna: it's ahead in Germany and builds card habits every month. Platform: the Mastercard and Paymentology platform is already paid for and earns nothing yet. Capacity: the Amazon Business pilot (October 2026) absorbs capacity, so the card slips without a committed slot.
- **Primary success metric the one number that defines success, from M3:** Active Card Usage Rate- 75% of activated cards used for at least one transaction within 30 days. Why: Shows early adoption and validates that customers are replacing debit cards with Riverty Mastercard.
- **Baseline rate today's rate of your primary metric, from your M3 data:** 50% Active Card Usage Rate
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** Guardrail Metric: BNPL Purchase Success Rate at partner merchants (92%)
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** +25 percentage points
- **Sample size per arm use the calculator in the builder, baseline + MDE:** 58 users per arm
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** Traffic Split: 50% Control / 50% Treatment.
Test Duration: 6 weeks
- **Significance threshold p < 0.05 is standard, explain any deviation:** 95% confidence (p < 0.05) with 80% statistical power

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** Today, after being approved for a Riverty Mastercard, customers must wait for their physical card before they can start using it. During this waiting period, Lena continues using her debit card for in-store purchases because Riverty is not immediately available through a digital wallet. As a result, money leaves her account instantly, she cannot benefit from the "Keep it first, pay later" experience, and early card adoption is delayed, contributing to a lower Active Card Usage Rate.
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** Instant Virtual Mastercard & Apple/Google Wallet, Simplified PRD (Your Riverty case)
Author: Me · Status: Draft · Target: High-Fidelity Prototype · Persona: Lena- A 32-year-old salaried employee in Cologne on a middling income with no real cushion, who shops mostly on her phone.

1. The Big Picture
Vision: Enable customers to start using their Riverty Mastercard instantly, making "Keep it first, pay later" available everywhere from day one.
Press release: Riverty Introduces Instant Virtual Mastercard—Start Shopping in Minutes, Not Days Berlin, Germany — Say goodbye to waiting for your card to arrive. Riverty is introducing the Instant Virtual Mastercard, allowing approved customers to add their card to Apple Pay or Google Wallet and start shopping immediately. Whether buying online or paying in-store, customers can now enjoy Riverty's signature "Keep it first, pay later" experience from the moment they're approved—wherever Mastercard is accepted. For shoppers like Lena, who often has to fall back on her debit card because Riverty isn't available in-store, this changes everything. Instead of paying upfront before deciding whether to keep an item, she can make purchases instantly with her Riverty Mastercard and enjoy the flexibility she's come to expect. By removing the wait between approval and first purchase, Riverty transforms from a checkout payment option into an everyday payment companion—making flexible payments faster, simpler, and always within reach.
Success metric: Active Card Usage Rate- 75% of activated cards used for at least one transaction within 30 days. Why: Shows early adoption and validates that customers are replacing debit cards with Riverty Mastercard.
Guardrail: The percentage of customers who successfully complete a purchase using Riverty BNPL at partner merchants should not decrease after the Mastercard launch.
2. The Details
User stories
As a newly approved Riverty customer, I want my virtual Mastercard to be available immediately so that I can start using it without waiting for a physical card.
As a customer, I want to add my Riverty Mastercard to Apple Pay or Google Wallet so that I can pay in-store and online immediately.
As a customer, I want to securely verify my identity before my virtual card is activated so that my account remains protected.
As a customer, I want to receive confirmation when my virtual card is activated so that I know it is ready to use.
As a customer, I want my virtual card to be available in real time after approval so that I can make my first purchase straight away.
As a customer, I want clear instructions for adding my card to my digital wallet so that I can complete the setup without confusion.
As a customer, I want to receive a notification when my card is successfully added to my wallet so that I know I can start paying immediately.
As a customer, I want to view my virtual card details and wallet status in the Riverty app so that I can easily manage my card.
As a customer, I want to receive real-time notifications after every transaction so that I can track my spending and detect any unexpected activity.
As a customer, I want to temporarily freeze or unfreeze my virtual card so that I can protect my account if my phone is lost or I suspect fraudulent activity.
Screens to build
Entry Point – Card Approved
Purpose: Inform the customer that their Riverty Mastercard is ready and encourage immediate action.
Screen Name
Congratulations! Your Riverty Mastercard is Ready
UI Elements
Success message: "You're approved!"
Virtual Mastercard preview
Buttons:
Add to Apple Pay / Google Wallet
View Card Details
Key benefits:
Use instantly
Shop online & in-store
No need to wait for your physical card
Primary CTA: Add to Wallet
Feature Core – Add to Apple Pay / Google Wallet
Purpose: Allow customers to securely provision their virtual card to their preferred digital wallet.
Screen Name
Add Your Card to Your Wallet
UI Elements
Virtual card preview
Apple Pay / Google Wallet selection
Secure identity verification prompt (if required)
Progress indicator
"Add to Wallet" button
Help link: Need help setting up?
Primary CTA: Confirm & Add Card
Success / Confirmation
Purpose: Confirm successful setup and encourage the customer's first purchase.
Screen Name
You're Ready to Pay
UI Elements
Success icon (✓)
Message:Your Riverty Mastercard has been added successfully.
Wallet confirmation
Suggested next action:
Start Shopping
Find Partner Merchants
Small reminder:Keep it first, pay later—wherever Mastercard is accepted.
Primary CTA: Start Shopping
Functional requirements
FR1 – Instant Virtual Card Generation
FR2 – Apple Pay & Google Wallet Provisioning
FR3 – Secure Customer Authentication
FR4 – Real-Time Card Activation
FR5 – Card Ready Confirmation
FR6 – Immediate Payment Readiness
FR7 – Wallet Provisioning Status
FR8 – Error Handling
Smart behaviors (Situation → Outcome)
Smart Behaviors (If → Then)
If a customer is successfully approved for a Riverty Mastercard, then the system generates a virtual Mastercard and makes it available within 30 seconds.
If the virtual Mastercard is generated successfully, then the system prompts the customer to add it to Apple Pay or Google Wallet.
If identity verification is required before wallet provisioning, then the system requests authentication before continuing.
If the customer successfully adds the card to Apple Pay or Google Wallet, then the system displays a confirmation message and sends a push notification.
If wallet provisioning fails, then the system displays the reason for the failure and provides an option to retry.
If the customer makes their first successful purchase using the Riverty Mastercard, then the system sends a real-time transaction notification and encourages continued card usage.
If the customer has not added the virtual card to a digital wallet within 24 hours of approval, then the system sends a reminder to complete wallet setup.
If the customer has activated the card but has not completed a transaction within 7 days, then the system sends a personalised reminder highlighting the benefits of using the Riverty Mastercard.
Technical constraints
No physical card fulfilment
No automatic wallet provisioning across multiple devices
3. The Logistics
Features out
Spending Analytics Dashboard
Multi-Currency Support
AI-Powered Spending Insights
Edge cases & safety guard
Must never store or transmit payment credentials outside Mastercard, Apple Pay, Google Wallet, and Riverty's approved secure infrastructure.
Safety Guard (Must NEVER Do)
Must never issue a virtual Mastercard before customer identity and eligibility are successfully verified.
Must never allow transactions using an inactive, blocked, or expired virtual card.
Must never expose the full card number, CVV, or sensitive payment credentials in notifications or unsecured screens.
Must never create duplicate virtual cards for the same approved application.
Must never store or transmit payment credentials outside Mastercard, Apple Pay, Google Wallet, and Riverty's approved secure infrastructure.
Decision log
Decision 1: Prioritise Instant Card Access Over Advanced Card Features
Decision 2: Support Digital Wallets Only
Evals
Accuracy
Target: ≥ 98% of eligible customers successfully generate and add their virtual Riverty Mastercard to Apple Pay or Google Wallet on their first attempt.
Time-on-Task
Target: ≤ 2 minutes for customers to complete the journey from card approval to successful wallet provisioning.
Safety
Target: 100% of virtual card activations require successful customer authentication, with 0 unauthorized card activations.
MoSCoW scope
Must: Instant Virtual Card Generation; Apple Pay & Google Wallet Provisioning; Secure Customer Authentication; Card Activation Confirmation; Real-Time Card Availability
Should: Wallet Setup Guide; Push Notification After Wallet Added; In-App Digital Card View; Sending Notifications after successful notification
Could: Automatic Wallet Provisioning; Device Management; Temporary Card Freeze
Won't (now): Spending analytics dashboards; Multi-currency support; AI-Powered Spending Insights
Builder hook: Build a working prototype based on this PRD. Use the User Story as the core flow, Functional Requirements as build constraints, and prioritize speed and clarity over visual complexity.
- **Isolation check, what has NOT changed? list everything identical between arms (app version, recommendation engine, notifications, onboarding). If something changed inadvertently, your test is compromised.:** Only the onboarding experience changed by introducing Instant Virtual Mastercard with Apple Pay and Google Wallet provisioning. All other variables remained unchanged, including the credit approval process, credit limits, pricing, repayment terms, merchant network, BNPL checkout experience, marketing campaigns, and eligibility criteria. This ensures that any change in the Active Card Usage Rate can be attributed to immediate digital card availability rather than other product or business changes.

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** We believe that introducing an Instant Virtual Mastercard with Apple Pay and Google Wallet for Lena, a 32-year-old salaried employee in Cologne with a middling income who shops primarily on her phone, will enable her to start using Riverty immediately after approval, replacing debit card usage for everyday purchases and making "Keep it first, pay later" available wherever Mastercard is accepted. We expect this to increase the Active Card Usage Rate to 75% of activated cards completing at least one transaction within 30 days, measured over a 6-week pilot. Throughout the experiment, we will protect the BNPL Purchase Success Rate at partner merchants, ensuring it does not fall below the current baseline of 92%.
- **Your shipping criteria (filled in):** ✅ GO
- Active Card Usage Rate ≥ 75%
- BNPL Purchase Success Rate ≥ 92%
- Wallet provisioning success ≥ 98%
- No critical production issues

🔄 ITERATE
- Active Card Usage Rate 65–74%
- Minor usability or provisioning issues
- Improve onboarding and retest

❌ NO-GO
- Active Card Usage Rate < 65%
- BNPL Purchase Success Rate < 92%
- Critical security or payment issues
- Pause rollout and redesign
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** The hardest parameter to define was the baseline Active Card Usage Rate because no historical data was provided. I assumed a 50% baseline, which changed the experiment design (MDE and sample size) but not the hypothesis that instant digital card access would increase early adoption.
