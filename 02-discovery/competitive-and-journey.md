# Competitive Analysis & Journey Map (Module 2)

## Responses
- **Role, who are you solving for? (the specific user segment or profile):** A 32-year-old salaried employee in Cologne on a middling income with no real cushion, who shops mostly on her phone.
- **Goal, what is this user ultimately trying to achieve?:** To pay only after she has decided to keep the item.
- **Friction, the main barrier (moment of misery) stopping them from succeeding:** In a shop, Riverty isn't offered, so she pays by debit and the money leaves her account immediately, before she knows whether she'll keep what she bought.
- **External tools, the outside platforms or tools the user is forced to use:** Klarna (app and checkout): the brief says she has it installed and uses it whenever it appears at checkout. This is the one most strongly supported.
PayPal (Pay in 3 / Pay in 30): also installed, and used as a fallback BNPL option. Also supported by the brief.
Her debit card: the likely forced choice in a shop, where Riverty isn't offered. The brief implies it, but doesn't state it.
Her phone browser and online shops: where she would buy later if she skips the in-store purchase
- **The process, the 3 to 5 manual steps the user takes to get the job done:** Find the item in the shop and realise Riverty isn't offered there.
Pay by debit, so the money leaves her account straight away, before she has decided to keep it.
Take it home and decide whether she wants to keep it.
Return it if she doesn't, going back to the shop or posting it.
Wait for the refund to reach her account, carrying the gap in the meantime with no cushion.
- **Core frustration, the exact moment the process feels most “broken”:** the moment she pays by debit in the shop.

The money leaves her account before she has decided to keep the item. That reverses the one thing she wants from pay-later, and she has no cushion to absorb it if she changes her mind.
- **The evidence, a specific quote or behavior from the research that proves this:** Her stated preference: she "prefers the money to leave her account only after she has decided to keep the item." This proves the want, and what you'd break at step 2.
- **Your journey map, a shareable link, or the map file you committed (e.g. journey-map.html):** <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Future-State Journey - Riverty Mastercard</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Inter',sans-serif;
}

body{
    background:#f5f8fc;
    color:#233043;
}

.container{
    max-width:1500px;
    margin:auto;
    padding:40px;
}

header{
    margin-bottom:35px;
}

header h1{
    font-size:46px;
    color:#16354b;
}

header p{
    margin-top:8px;
    font-size:22px;
    color:#4c6477;
}

.timeline{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:22px;
    position:relative;
}

.card{
    border-radius:22px;
    padding:24px;
    color:#183247;
    box-shadow:0 10px 24px rgba(0,0,0,.08);
    position:relative;
}

.card:not(:last-child)::after{
    content:"➜";
    position:absolute;
    right:-18px;
    top:35px;
    font-size:30px;
    color:#7c8794;
}

.stage{
    width:52px;
    height:52px;
    border-radius:50%;
    color:#fff;
    display:flex;
    justify-content:center;
    align-items:center;
    font-size:22px;
    font-weight:bold;
    margin-bottom:16px;
}

.purple{
    background:#efe8ff;
}
.purple .stage{
    background:#6a39ff;
}

.green{
    background:#e8f8ed;
}
.green .stage{
    background:#16a765;
}

.orange{
    background:#fff1df;
}
.orange .stage{
    background:#f68b1f;
}

.blue{
    background:#e8f3ff;
}
.blue .stage{
    background:#2979ff;
}

h2{
    margin-bottom:6px;
    font-size:28px;
}

.subtitle{
    color:#65768a;
    margin-bottom:22px;
}

.section{
    background:white;
    border-radius:14px;
    padding:14px;
    margin-top:14px;
}

.section h4{
    margin-bottom:6px;
    color:#193b5d;
}

.section p{
    line-height:1.5;
    color:#526577;
}

.footer{
    margin-top:40px;
    background:white;
    border-radius:20px;
    padding:28px;
    box-shadow:0 8px 20px rgba(0,0,0,.08);
}

.footer h2{
    margin-bottom:20px;
}

.advantages{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.adv{
    background:#f4f9ff;
    border-left:6px solid #2979ff;
    padding:18px;
    border-radius:14px;
}

.adv h3{
    margin-bottom:8px;
    color:#18476b;
}

@media(max-width:1100px){

.timeline{
grid-template-columns:1fr;
}

.card::after{
display:none;
}

.advantages{
grid-template-columns:1fr;
}

header h1{
font-size:34px;
}

}
</style>

</head>

<body>

<div class="container">

<header>
<h1>Future-State Journey: Riverty Mastercard</h1>
<p><strong>Keep it first, pay later — anywhere</strong></p>
</header>

<div class="timeline">

<div class="card purple">

<div class="stage">1</div>

<h2>Discover Riverty Everywhere</h2>

<div class="subtitle">From awareness to activation</div>

<div class="section">
<h4>User Action</h4>
<p>Apply digitally → Instant approval and wallet-ready Mastercard.</p>
</div>

<div class="section">
<h4>Internal State</h4>
<p>Curious but cautious → Feels confident trying Riverty beyond checkout.</p>
</div>

<div class="section">
<h4>Pain Point Addressed</h4>
<p>Riverty only appears at selected merchant checkouts.</p>
</div>

</div>

<div class="card green">

<div class="stage">2</div>

<h2>Use Anywhere</h2>

<div class="subtitle">Online and in-store shopping</div>

<div class="section">
<h4>User Action</h4>
<p>Pay anywhere → Money leaves only after deciding to keep purchases.</p>
</div>

<div class="section">
<h4>Internal State</h4>
<p>Relieved and in control → No pressure from immediate debit.</p>
</div>

<div class="section">
<h4>Pain Point Addressed</h4>
<p>Physical stores previously forced immediate debit payment.</p>
</div>

</div>

<div class="card orange">

<div class="stage">3</div>

<h2>Manage Simply</h2>

<div class="subtitle">One place for everything</div>

<div class="section">
<h4>User Action</h4>
<p>View purchases together → Track and settle repayments easily.</p>
</div>

<div class="section">
<h4>Internal State</h4>
<p>Organised and reassured → Always knows what's due next.</p>
</div>

<div class="section">
<h4>Pain Point Addressed</h4>
<p>Payments are fragmented across multiple merchants and providers.</p>
</div>

</div>

<div class="card blue">

<div class="stage">4</div>

<h2>Make Riverty the Default</h2>

<div class="subtitle">An everyday relationship</div>

<div class="section">
<h4>User Action</h4>
<p>Use Riverty Mastercard daily → Earn convenience and flexibility.</p>
</div>

<div class="section">
<h4>Internal State</h4>
<p>Trusting and loyal → Riverty becomes the preferred payment brand.</p>
</div>

<div class="section">
<h4>Pain Point Addressed</h4>
<p>No compelling reason to choose Riverty over Klarna or PayPal.</p>
</div>

</div>

</div>

<div class="footer">

<h2>Competitive Advantages over the Manual Workaround</h2>

<div class="advantages">

<div class="adv">
<h3>🌍 Pay Later Everywhere</h3>
<p>No dependence on partner merchants. Use Riverty Mastercard anywhere Mastercard is accepted.</p>
</div>

<div class="adv">
<h3>📱 One Repayment Hub</h3>
<p>Track every purchase, due date and repayment from one Riverty experience.</p>
</div>

<div class="adv">
<h3>❤️ Everyday Relationship</h3>
<p>Builds daily engagement and loyalty instead of being only a checkout payment option.</p>
</div>

</div>

</div>

</div>

</body>
</html>
