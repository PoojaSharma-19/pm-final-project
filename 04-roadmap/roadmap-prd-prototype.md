# Feature Roadmap, Module 4 · Your Riverty case

**Team:** the team named in your case

## Strategic anchors
- **Persona:** A 32-year-old salaried employee in Cologne on a middling income with no real cushion, who shops mostly on her phone.
- **Primary metric:** Active Card Usage Rate- 75% of activated cards used for at least one transaction within 30 days. Why: Shows early adoption and validates that customers are replacing debit cards with Riverty Mastercard.
- **Moment of misery:** In a shop, Riverty isn't offered, so she pays by debit and the money leaves her account immediately, before she knows whether she'll keep what she bought.
- **Guardrail:** The percentage of customers who successfully complete a purchase using Riverty BNPL at partner merchants should not decrease after the Mastercard launch.

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| R1  | 5 | 5 | Major Project | Now | This is the core value proposition of the Riverty Mastercard. It directly solves Lena's biggest pain point—paying before deciding to keep an item—and clearly differentiates Riverty from traditional debit cards. However, it requires significant work across payments, risk, and settlement processes. |
| R2  | 5 | 3 | Major Project | Next | Automatically matching refunds with outstanding repayments improves customer trust and reduces payment friction after returns. It requires integrations with merchants and refund processing, making implementation moderately complex. |
| R3  | 4 | 3 | Major Project | Now | Enables existing Riverty customers to apply in minutes using pre-filled information, reducing onboarding friction and increasing activation. It requires integration with identity verification, credit assessment, and card issuance systems. |
| R4  | 3 | 2 | Fill-In | Later | Automatically settling balances on the due date helps customers avoid missed payments and reminder fees. It is simple to implement and reduces operational costs while improving customer trust. |
| R5  | 2 | 5 | Time Sinker | Cut | Providing merchants with anonymised spending insights could strengthen partnerships but offers little immediate value to Lena. The feature requires significant data engineering and reporting capabilities, making it unsuitable for an MVP. |
| R6  | 4 | 2 | Quick Win | Now | Offers exclusive rewards when shopping with Riverty partner merchants, encouraging repeat usage while supporting Riverty's merchant-first strategy. Suitable after the core proposition has been validated. |
| R7  | 4 | 2 | Quick Win | Next | Smart reminders before the return window closes and before payment is due help customers decide whether to keep or return purchases, reinforcing the "Keep it first, pay later" proposition with minimal development effort. |
| R8  | 4 | 2 | Quick Win | Now | Provides immediate access to the card through Apple Pay or Google Pay after approval, encouraging faster activation and everyday usage without waiting for a physical card. |

## Roadmap
### NOW, this sprint
- **R1 **, This is the core value proposition of the Riverty Mastercard. It directly solves Lena's biggest pain point—paying before deciding to keep an item—and clearly differentiates Riverty from traditional debit cards. However, it requires significant work across payments, risk, and settlement processes.
- **R3 **, Enables existing Riverty customers to apply in minutes using pre-filled information, reducing onboarding friction and increasing activation. It requires integration with identity verification, credit assessment, and card issuance systems.
- **R6 **, Offers exclusive rewards when shopping with Riverty partner merchants, encouraging repeat usage while supporting Riverty's merchant-first strategy. Suitable after the core proposition has been validated.
- **R8 **, Provides immediate access to the card through Apple Pay or Google Pay after approval, encouraging faster activation and everyday usage without waiting for a physical card.

### NEXT, the following sprints
- **R2 **, Automatically matching refunds with outstanding repayments improves customer trust and reduces payment friction after returns. It requires integrations with merchants and refund processing, making implementation moderately complex.
- **R7 **, Smart reminders before the return window closes and before payment is due help customers decide whether to keep or return purchases, reinforcing the "Keep it first, pay later" proposition with minimal development effort.

### LATER, backlog
- **R4 **, Automatically settling balances on the due date helps customers avoid missed payments and reminder fees. It is simple to implement and reduces operational costs while improving customer trust.

### ✂ Cut List
- **R5 **, Providing merchants with anonymised spending insights could strengthen partnerships but offers little immediate value to Lena. The feature requires significant data engineering and reporting capabilities, making it unsuitable for an MVP.
