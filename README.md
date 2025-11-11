# credit-utilization-helper

A simple browser-based tool to calculate credit card utilization and plan how to apply extra payments.

👉 Try it live: https://cybernomadx.github.io/credit-utilization-helper/

---

## What it does

- Shows **per-card** and **overall** utilization
- Calculates how much to pay on each card to reach a **target utilization %** (default 30%)
- Suggests how to allocate a lump-sum payment across cards, with two modes:
  - **Focus on score** – pay highest-utilization cards first
  - **Quick wins** – pay the smallest amounts needed to bring cards down to target first
- Optional: use leftover money to pay down the **highest-utilization** card after targets are hit
- Dark mode UI

---

## Privacy & data

This tool is intentionally simple and privacy-friendly:

- It runs entirely in your browser. There is **no backend, no login, and no account system**.
- **By default, nothing is saved**. If you close or refresh the page, your entries are gone.
- If you turn on **“Save my data on this device”**, the app uses your browser’s `localStorage` to remember:
  - Card names (can be generic)
  - Limits and balances
  - Target utilization %
  - Allocation strategy settings
  - “Use remainder” preference
  - Optional “available payment” amount
- This data:
  - Stays on **your device**, in **this browser** only
  - Is **never uploaded** to any server by this tool

For safety:

- Don’t enter full card numbers, CVV/CVC, bank logins, Social Security numbers, or similar sensitive info.
- Card names can be something like “Card 1”, “Blue Visa”, or “Store card” — whatever you recognize.

If you’re using a shared or public device, keep saving turned off, or use the **“Clear saved data”** button before you leave.

---

## How to use

1. For each card, enter:
   - A card name (can be generic)
   - Credit limit
   - Current balance
2. Set your **target utilization %** (default 30%).
3. (Optional) Enter how much you can pay in total right now.
4. Choose an **allocation strategy**:
   - *Focus on score* or *Quick wins*
5. Click **Calculate**:
   - See per-card and total utilization
   - See “Pay to target” amounts per card
   - If you entered a lump-sum amount, see a suggested payment order (which cards to pay and roughly how much)

---

## Tech details

- Static single-page app: plain **HTML, CSS, and JavaScript**
- Hosted on **GitHub Pages**
- Uses `localStorage` only when the user enables the “Save my data on this device” option

---

Made by CyberNomadx.
