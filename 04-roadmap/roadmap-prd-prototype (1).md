# Roadmap, PRD & Prototype (Module 4)

## Your strategic anchors
- **Persona (M2), who are you solving for?:** A 32-year-old salaried employee in Cologne on a middling income with no real cushion, who shops mostly on her phone.
- **Primary success metric (M3), your leading indicator:** Active Card Usage Rate- 75% of activated cards used for at least one transaction within 30 days. Why: Shows early adoption and validates that customers are replacing debit cards with Riverty Mastercard.
- **Moment of misery (M2), the specific friction blocking the goal:** In a shop, Riverty isn't offered, so she pays by debit and the money leaves her account immediately, before she knows whether she'll keep what she bought.
- **Guardrail metric (M3), what must not drop or break:** The percentage of customers who successfully complete a purchase using Riverty BNPL at partner merchants should not decrease after the Mastercard launch.

## Scan the backlog & set a human baseline
- **My instinctive “quick wins” before touching the AI (2 to 3 feature IDs + why):** R6 - it will give reward to customers
R8 - it will increase the active Riverty cards

## Audit, override & decide
- **Where did you override the AI? (feature + old vs. new score + why):** Merchant Partner Rewards & Cashback + 4
new score is 3 + Although rewards may encourage spending, they do not directly solve Lena's primary pain point of paying before deciding to keep a purchase. Launching rewards in the MVP could also distort the experiment by making it unclear whether customers adopted the Riverty Mastercard because of the core value proposition or because of incentives. I prioritized validating the "Keep it first, pay later" proposition first and moved rewards to a later phase.
- **Did the AI over-value a Sales/Eng request your M2 interviews don’t support?:** Yes. The AI over-valued the "Merchant Partner Rewards & Cashback" feature by scoring it as a Quick Win (Value 4) and prioritising it for the "Now" roadmap. My Module 2 persona interviews and problem statement did not indicate that rewards or cashback were key motivations for Lena. Instead, the strongest customer need was the ability to "pay only after deciding to keep the item" and to use Riverty in physical stores. Introducing rewards in the MVP could also bias the experiment, making it difficult to determine whether customers adopted the Riverty Mastercard because of its core value proposition or because of incentives. Therefore, I moved this feature to the "Later" phase and focused the MVP on features that directly address Lena's primary pain point and improve the Active Card Usage Rate.
- **Did it underweight something your M3 cohort/funnel data strongly supports?:** Yes. The AI slightly underweighted the value of "Instant Virtual Mastercard & Mobile Wallet" (R8). My Module 3 funnel focuses on increasing the Active Card Usage Rate, with success measured by 75% of activated cards completing at least one transaction within 30 days. Immediate digital card provisioning removes the delay between approval and first use, making it more likely that customers use the Riverty Mastercard for their next purchase instead of reverting to their debit card. I therefore increased its value score from 4 to 5 and prioritised it in the "Now" roadmap because it has a direct impact on the leading indicator we are trying to improve.

## Generate your interactive roadmap
- **My “Now” lane (this sprint), the 2 to 3 quick wins I’ll build first:** R1 – Decision-Window Settlement
R3 – Fast In-App Application & Instant Approval
R8 – Instant Virtual Mastercard & Mobile Wallet
- **What I cut, and the “no” I’m protecting the scope from:** Merchant Analytics & Spending Insights Dashboard
- **Prototype/roadmap screenshot link (paste into your deliverables):** <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Riverty Mastercard - Feature Roadmap</title>
    <style>
        :root {
            --bg-color: #f8fafc;
            --text-main: #0f172a;
            --text-sub: #64748b;
            --now-color: #10b981;
            --now-bg: #ecfdf5;
            --next-color: #2563eb;
            --next-bg: #eff6ff;
            --later-color: #f59e0b;
            --later-bg: #fffbeb;
            --cut-color: #ef4444;
            --cut-bg: #fef2f2;
            --card-bg: #ffffff;
            --border-radius: 8px;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            padding: 24px;
        }

        .roadmap-container {
            max-width: 1400px;
            margin: 0 auto;
            background: #ffffff;
            border-radius: 12px;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05), 0 2px 4px -1px rgba(0, 0, 0, 0.03);
            padding: 24px;
        }

        /* Header Section */
        .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
            padding-bottom: 24px;
            border-bottom: 1px solid #e2e8f0;
        }

        .brand-zone {
            display: flex;
            align-items: center;
            gap: 16px;
        }

        .logo {
            font-size: 32px;
            font-weight: 800;
            color: #0f172a;
            letter-spacing: -0.5px;
        }

        .title-area {
            border-left: 2px solid #e2e8f0;
            padding-left: 16px;
        }

        .title-area h1 {
            font-size: 24px;
            font-weight: 700;
            color: #1e293b;
        }

        .title-area p {
            font-size: 14px;
            color: var(--text-sub);
            margin-top: 2px;
        }

        .metrics-zone {
            display: flex;
            gap: 16px;
        }

        .metric-card {
            background: #f1f5f9;
            padding: 12px 16px;
            border-radius: var(--border-radius);
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .metric-icon {
            font-size: 24px;
        }

        .metric-info data {
            display: block;
            font-size: 12px;
            color: var(--text-sub);
            font-weight: 600;
            text-transform: uppercase;
        }

        .metric-info span {
            font-size: 13px;
            color: #334155;
            font-weight: 500;
        }

        /* Timeline Tracker Line */
        .timeline-tracker {
            display: flex;
            margin: 24px 0;
            position: relative;
            padding: 0 12px;
        }

        .timeline-segment {
            flex: 1;
            height: 4px;
            position: relative;
        }

        .timeline-segment::before {
            content: '';
            position: absolute;
            left: 0;
            right: 0;
            top: 0;
            height: 100%;
        }

        .timeline-segment.now::before { background-color: var(--now-color); }
        .timeline-segment.next::before { background-color: var(--next-color); }
        .timeline-segment.later::before { background-color: var(--later-color); }
        .timeline-segment.cut::before { background-color: var(--cut-color); }

        .timeline-dot {
            width: 14px;
            height: 14px;
            border-radius: 50%;
            position: absolute;
            top: -5px;
            left: 50%;
            transform: translateX(-50%);
            border: 3px solid #ffffff;
            box-shadow: 0 0 0 2px currentColor;
        }

        .timeline-segment.now { color: var(--now-color); }
        .timeline-segment.next { color: var(--next-color); }
        .timeline-segment.later { color: var(--later-color); }
        .timeline-segment.cut { color: var(--cut-color); }

        /* Board Columns Grid */
        .board-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 16px;
            align-items: start;
        }

        .column {
            border-radius: var(--border-radius);
            padding: 16px;
            display: flex;
            flex-direction: column;
            gap: 12px;
            min-height: 450px;
        }

        .column.now { background-color: var(--now-bg); }
        .column.next { background-color: var(--next-bg); }
        .column.later { background-color: var(--later-bg); }
        .column.cut { background-color: var(--cut-bg); }

        .column-header {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .column-icon {
            width: 32px;
            height: 32px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ffffff;
            font-size: 16px;
        }

        .now .column-icon { background-color: var(--now-color); }
        .next .column-icon { background-color: var(--next-color); }
        .later .column-icon { background-color: var(--later-color); }
        .cut .column-icon { background-color: var(--cut-color); }

        .column-title h2 {
            font-size: 16px;
            font-weight: 700;
        }

        .column-title p {
            font-size: 13px;
            color: var(--text-sub);
        }

        .column-focus {
            font-size: 13px;
            color: #475569;
            line-height: 1.4;
            padding-bottom: 8px;
            border-bottom: 1px solid rgba(0,0,0,0.06);
        }

        /* Feature Cards */
        .feature-card {
            background-color: var(--card-bg);
            border-radius: 6px;
            padding: 14px;
            display: flex;
            align-items: flex-start;
            gap: 12px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
            cursor: pointer;
            transition: transform 0.15s ease, box-shadow 0.15s ease;
            position: relative;
        }

        .feature-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 6px -1px rgba(0,0,0,0.08);
        }

        .card-tag {
            font-size: 13px;
            font-weight: 700;
            min-width: 24px;
        }

        .now .card-tag { color: var(--now-color); }
        .next .card-tag { color: var(--next-color); }
        .later .card-tag { color: var(--later-color); }
        .cut .card-tag { color: var(--cut-color); }

        .card-icon {
            font-size: 18px;
            margin-top: -2px;
        }

        .card-content {
            flex: 1;
        }

        .card-content h3 {
            font-size: 13px;
            font-weight: 700;
            color: #1e293b;
            margin-bottom: 2px;
        }

        .card-content p {
            font-size: 12px;
            color: var(--text-sub);
            line-height: 1.35;
        }

        .card-arrow {
            color: #cbd5e1;
            font-weight: bold;
            font-size: 14px;
            align-self: center;
        }

        /* Responsive Breakpoints */
        @media (max-width: 1024px) {
            .board-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .timeline-tracker {
                display: none;
            }
        }

        @media (max-width: 640px) {
            .board-grid {
                grid-template-columns: 1fr;
            }
            .header {
                flex-direction: column;
                align-items: flex-start;
            }
            .metrics-zone {
                width: 100%;
                flex-direction: column;
            }
        }
    </style>
</head>
<body>

    <div class="roadmap-container">
        <!-- Header Section -->
        <header class="header">
            <div class="brand-zone">
                <div class="logo">Riverty</div>
                <div class="title-area">
                    <h1>Riverty Mastercard – Feature Roadmap</h1>
                    <p>Keep it first, pay later. Everywhere.</p>
                </div>
            </div>
            
            <div class="metrics-zone">
                <div class="metric-card">
                    <span class="metric-icon">📊</span>
                    <div class="metric-info">
                        <data>Primary Metric</data>
                        <span><strong>Active Card Usage Rate</strong><br>75% of activated cards used for at least one transaction within 30 days.</span>
                    </div>
                </div>
                <div class="metric-card">
                    <span class="metric-icon">👥</span>
                    <div class="metric-info">
                        <data>Team</data>
                        <span>5 Developers</span>
                    </div>
                </div>
            </div>
        </header>

        <!-- Timeline Segment Line -->
        <div class="timeline-tracker">
            <div class="timeline-segment now"><div class="timeline-dot"></div></div>
            <div class="timeline-segment next"><div class="timeline-dot"></div></div>
            <div class="timeline-segment later"><div class="timeline-dot"></div></div>
            <div class="timeline-segment cut"><div class="timeline-dot"></div></div>
        </div>

        <!-- Main Product Board Layout -->
        <main class="board-grid">
            
            <!-- NOW Column -->
            <section class="column now">
