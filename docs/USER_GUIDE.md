# User guide

> © 2026 TCGPro. All rights reserved.

## The everyday loop

1. **Buy** → *Add cards*: record the purchase and its cards.
2. **Price** → open the card from *Inventory*, then *Calculate* the recommended prices. Click *Use recommended* (or type your own price) for each marketplace.
3. **List** → copy the fields from the *Listing helper* into Cardmarket, or press **List on eBay** on a card to upload it to eBay (when eBay is connected). Set the status to *Listed*.
4. **Sell** → *Record sale* when an order comes in. Profit is worked out from what you paid for the oldest copy first. If the card is also listed on the other marketplace, you get a reminder to update that listing.
5. **Review** → check *Aging* for slow stock, the *Dashboard* for performance, and *Reports* for PDFs.

---

## Your free trial and subscription

1. **Starting.** The first time you open TCGPro, type your email and press *Start my free trial*. You get 14 days with everything working. No card is needed. You get one trial per person and per computer.
2. **During the trial** a bar at the top shows the days left. *Subscribe* is there any time you want it.
3. **Subscribing.** Choose *Yearly* or *Monthly*, press *Continue to payment*, and pay on the secure payment page that opens in your browser. Come back to TCGPro: it notices the payment by itself (or press *I have paid, check now*).
4. **Managing it.** *Settings › About › Subscription* shows your plan and renewal date, and has *Update payment method*, *Cancel subscription* and *Invoices and details*. If you cancel, TCGPro keeps working until the end of the period you paid for.
5. **Your licence key** is shown there too. Keep it: it lets you use TCGPro on a new computer (up to 2 computers at a time). Choose *I already have a licence key* on the first screen of the new computer.
6. **If the trial or subscription ends, TCGPro does not lock.** It opens *read-only*: you can look at everything and export it (Reports as PDF or Excel, backups), but you cannot add or change things until you subscribe again. Your data is never deleted or held back.
7. **If a payment fails,** TCGPro keeps working for a week while the payment is retried, and the top bar asks you to update your payment method.

People who bought TCGPro earlier with a licence key keep it. Their licence is not a subscription and does not end.

---

## Syncing your Cardmarket stock

1. Press **Sync Cardmarket** (Dashboard) or **Sync from Cardmarket** (Inventory, top right). In the Mac app everything happens inside TCGPro: Cardmarket is read in the background and the progress is shown in the sync window. There is nothing to install.
2. The first time, and now and then afterwards, Cardmarket may ask for you. A small Cardmarket window then appears by itself: log in, or tick Cardmarket's "Verify you are human" box. The sync carries on by itself right after, and the window disappears again. TCGPro remembers your Cardmarket login.
3. The stock for all three games is read automatically. Keep TCGPro open until the window says *Sync finished*.
   (If you open TCGPro from a normal browser instead of the Mac app, the Cardmarket browser extension is used, as before: the app guides you through installing it.)
   (The Windows version is not released yet. The steps below apply to it when it is.)   **On Windows** the sync uses the Edge/Chrome extension, not a built-in window. One-time install: open `edge://extensions` (Chrome: `chrome://extensions`), turn on **Developer mode**, click **Load unpacked** and choose the folder `%APPDATA%\TCGBusinessSuite\cardmarket-sync-extension` (TCGPro keeps this copy up to date by itself and it survives moving or updating the app; the Cardmarket page shows the exact folder and has *Open extensions page* and *Show the folder* buttons). Keep your normal Edge/Chrome signed in to Cardmarket. First run of the Windows app: if SmartScreen warns, click **More info**, then **Run anyway**; unzip the app anywhere except Program Files and double-click `TCGPro.exe`.
4. **Review changes**:
   - *On Cardmarket but not in your inventory*: tick entries (or none for all), then use **Add to inventory…** and choose how to set their cost.
   - *Not matched to the catalog*: refresh price data in Settings, then sync again.

The first sync shows all your current Cardmarket stock as "not in your inventory". After you add it, later syncs only report what changed.

## Adding cards (Add cards)

1. **Purchase:** fill in these fields.
   - **Date**.
   - **Bought from:** an individual, a private collection, a shop or a wholesaler.
   - **Source name**.
   - **Seller contact** (optional). It is stored encrypted.
   - **Type:** individual cards or a collection purchase.
   - **Total paid**.
   - For collections, optionally what the **seller asked**.
2. **Cards:** search by name or collector number, for example `OP01-001`, `MEW 144`, `OGN 056` or `Charizard ex`. You can filter by game.
   - Each result shows the set (when known), the number, the Cardmarket product ID, the date it was added and the current trend price. These help you pick the right version.
   - **Not in the catalog?** Choose *Add it manually*. You can later link it to the catalog from *Settings › Price data & catalog › Manual cards*, or from the card's page. Its stock, lots, sales and manual prices move with it.
   - For each line, set the condition, language, foil and quantity. Under *Notes / defects / more* you can add the edition, another attribute (Reverse Holo, Alt Art…), defects and notes.
3. **How to split the cost.** Every copy needs a cost, so that your profit can be worked out:
   - *By market value* (recommended): the total is split in proportion to each card's market value. Every card needs a usable price.
   - *Equally per copy*.
   - *I'll enter the cost per line*: the line costs must add up to the total.
4. **Check & save** shows an indicative market value against what you pay.

Grouping is automatic. The same card in the same condition, language, edition, foil, signed and altered state goes into one inventory entry. Copies that differ in any of these get a separate entry.

### Missing or unreliable prices

- A card is flagged **! Missing** when Cardmarket has no trend price for it (for foils, no foil trend).
- It is flagged **! Stale** when the data is too old for its value.
- When that happens, the app stops the affected calculation and asks you to **Enter value**.
- What you type is saved as a *Manual* value with the date. It is never shown as market data, and it stays valid for 30 days (you can change this).
- **▲ Volatile** means the 1-day average is far from the trend. Calculations still run, but check before you trust the number.

---

## Inventory

- Tabs per game, plus *All games*.
- The search box matches the name, collector number or set.
- **Filters** can be combined: condition, language, edition, foil, listing status, quantity range, average cost range and market price range.
- **Trend** is the current Cardmarket reference. *▲ old* means the price data is more than 7 days old.
- Tick several cards and use *Recalculate recommended prices* to reprice them in one go.

### A card's page

- **Market reference:** the price, its source and timestamp, the lowest listing, the 1/7/30-day averages and the trend history (recorded from the day you hold the card). You can override it with a manual value.
- **Recommended prices** are calculated separately for Cardmarket and eBay. Each shows every step:
  - reference × condition factor × strategy %;
  - optionally undercutting the lowest listing;
  - rounding and the minimum price;
  - for eBay, the optional **tracked-shipping adjustment** you set in Settings (it starts at €0);
  - the fee estimate, the cost of the oldest copy, and the expected profit — or the **expected LOSS**, shown in red. There is no minimum-profit block; the decision is yours.

  A saved recommendation never changes by itself. If the market moves 5% or more afterwards, a notice suggests recalculating.
- **Your asking price** per marketplace changes only when you click *Use recommended* or *Set*.
- **Listing helper:** ready-to-copy fields for Cardmarket, and for eBay a title of up to 80 characters, the item specifics and a description.
  - Condition is translated to Cardmarket's and eBay's grading terms as a suggestion. Check it against their guides.
  - Photos: eBay allows some listings to go live without photos, with photos added later, but not every category does. If eBay asks for photos, add them; the app does not work around that.
- **Where your copies came from (oldest first):** the oldest purchase is used up first when you sell.
- **Sales:** each sale can be voided, which restores the stock and lots exactly.
- **Edit details:** change the condition or attributes. If an identical entry already exists, the two are merged together with their history.

---

## Evaluate deals

- **Quick deal calculator:**
  1. Add the card(s) on offer and the asking price per line.
  2. You get the market value, a resale price on each marketplace (from your strategy), the fees, and the profit if you buy at the asking price and resell there.
- **Collection analysis:**
  1. Add the collection's cards and the seller's total asking price.
  2. You get the estimated market value, the difference, and the asking price as a % of market value. Cards without a usable price are flagged, and the total says it is incomplete.
  3. *Save evaluation* keeps it for later.
  4. *Bought it → record acquisition* copies the cards into *Add cards*.

---

## Sales

Every sale is in one list, newest first. Imported spreadsheet sales are marked *from Excel*.

Cardmarket sales can be pre-filled for you: press Scan sales, check the orders (edit or void if needed) and print the packing list. The stock sync itself never creates sales. Orders are matched by Cardmarket order number, so nothing is added twice.

**To record a sale:**
1. **Sales › ＋ Record sale**.
2. Type the card name and pick it from your stock.
3. Fill in marketplace, quantity, price and fees, then Save.

If the card isn't in your inventory, just keep the name you typed and Save. It's recorded with no stock change and no card cost, and marked *not from inventory*.

**Price and fees, the same way every time:**
- **Price** = what the buyer paid, including the shipping they paid.
- **Fees & costs** = what you paid: marketplace commission + postage + packaging.

**Mistakes:** **Void** undoes a sale. For sales from inventory, stock and costs are restored exactly. Sales not from inventory also have **Edit**.

After a sale of a card that's also listed on the other marketplace, a reminder appears so you can update that listing and avoid overselling.

## Aging

- Shows how long your copies have been held, and lists slow-moving cards: held 90+ days with no sale in 90 days. You can change this.
- **Suggested price cuts** are 5% after 60 days, 10% after 120 days and 20% after 180 days. You can change them.
- A suggestion applies only when you click **Apply**, and then only to the app's asking price. Update the listing on the marketplace yourself.

---

## Dashboard

- Choose the **date range** (presets or custom), **game** and **marketplace** at the top.
- **Widgets** (top right): show or hide widgets, choose line, bar or table where offered, set daily, weekly or monthly grouping for the trend, and set the default date range.
- **Move things around** (top right): drag the figures and widgets into the order you like. The layout is saved.
- Every chart has *Show as table*.

The widgets available are:
- Key figures: revenue, fees, realized profit, cards sold, stock copies, stock at cost, indicative market value, acquisition spend.
- Revenue & profit over time.
- Sales by marketplace.
- Sales by game.
- Best-selling cards.
- Inventory aging.
- Acquisition performance: what each purchase has earned back so far.
- Inventory by game.
- Business value and profit, and business events.
- Loose ends to sort out, stock that is stuck (90+ days), and this month against last month.
- Optional extras (use *＋ Add widget*): profit by day of the week, fees by marketplace, top buyers, today's to-do, goal progress, price movers and cards listed more than you own.

## Your own layout on every page

Sales, Inventory, Add cards, Acquisitions, Evaluate deals, Goals, Stock check, Bulk lots, Finance, Reports, Grading, Inventory aging and the eBay plan all have an **Edit layout** button at the top.
- Drag a panel to move it, press **−** to hide it, press **＋ Add widget** to bring a hidden panel back or to add an optional widget for that page, then press **Done**.
- The layout is remembered on this computer, separately for each language.

## Language

Settings has a **Language** list (English, Français, Deutsch, Español, Italiano, Português, Nederlands). The program reloads in that language. Your own data (card names, notes, dates) is never translated. The translations are machine translations with hand corrections: if anything reads badly, tell us through the contact form at https://mytcgpro.com/pages/contact.

---

## Reports

1. Tick the sections you want:
   - Business performance
   - Profitability
   - Sales log
   - Inventory
   - Acquisitions
   - Market valuation
   - Aging
2. Choose the period, game and marketplace.
3. Click **Generate PDF**.

---

## Goals

1. Press **New goal** and pick a template (for example a profit target, a number of sales, or a stock level). Or choose *Build your own goal*.
2. Type the target and the date. TCGPro tracks it against your real sales and stock and shows whether you are *Ahead of pace*, *On track*, *Behind* or *Reached*.
3. **Refresh** reads eBay again (when it is connected) and the latest Cardmarket data from the last sync, then updates every goal. *Where you stand* shows how many of your cards are listed on Cardmarket and on eBay and how many are not listed anywhere. Refresh opens nothing and changes none of your stock, prices or listings. If Cardmarket data is old, a note says so: run the Cardmarket SYNC from the Dashboard when you want it fresh.
   Right under each goal, **Next objectives** proposes what to aim for next, with the cards involved. These are suggestions to read: they do not open other screens, and nothing changes unless you do it yourself.
4. To stop tracking a goal, press the remove button on it. Your sales and stock are not touched.

---

## Stock check

Your stock mirrors Cardmarket. A card you sold on eBay or Vinted stays "in stock" until you remove its Cardmarket listing. This screen lists such cards so you do not sell the same card twice.

1. Open **To check**. Each card shows what you sold, when, and how likely it is that the listing is out of date (*Likely sold*, *Check*, *Different grade*).
2. If you really sold it, press **Sold: remove on Cardmarket**. It moves to the **Remove on Cardmarket** tab; press *Open on Cardmarket*, remove the listing there, then sync.
3. If you still have the card, press **I still have it**. It moves to **I still have them** and stops being flagged.
4. Done items stay under **Done** for your records.

---

## Bulk lots

Turns cheap cards into lots (for example 100 cards in one eBay listing) so they stop clogging your stock.

1. Choose the game, the **cards per lot** and the **accepted loss**.
2. **Lots to sell** shows each suggested lot with the value of its cards, a price with free shipping that covers your postage, and what you keep.
3. For a lot press **List (CSV)** to get the card list, or **eBay text** to copy the title and description. Take your own photo, list it on eBay, then remove those singles from Cardmarket.
4. Press **Set aside** so those copies stay out of the next lots. When the lot sells, press **Mark sold** under *Already set aside*. Changed your mind? **Release the copies** gives them back.
5. **Hot decks vs your stock** shows how much of each popular deck you own (for games where deck lists are available).

---

## Shipping labels

Print the buyers' addresses on small labels, several to an A4 sheet, instead of one per page.

1. Type your return address once (it is printed small in the corner of every label).
2. On eBay, copy the buyer's address and paste it into **Add the buyers' addresses**. To add several at once, leave an empty line between them. Press **Add to the list**.
3. Tick the labels to print. Each label is 13 × 6 cm: **paper sideways** fits 6 per sheet, **paper upright** fits 4.
4. Using a sheet you already started? Choose **First label goes in position** so the first free place is used and no paper is wasted.
5. Press **Make the PDF**, open it and print at 100% (actual size, not "fit to page"). Printed labels move to *Printed*, where **Print again** brings one back.

The addresses stay on this computer: they are not sent anywhere and not written to the history. Printed labels are deleted after 30 days.

## Finance

- **Overview**: the value of the whole business (cash plus every card, at your asking prices and at market value) minus what the partners put in. Try a price cut on everything listed to see where profit would turn into a loss.
- **Expenses**: supplies, grading, postage you pay, software and so on. Cards you buy to resell belong in *Add cards*, not here, otherwise they are counted twice.
- **Partner capital**: money or cards each partner put in. Money counts towards cash; items count only towards what was invested.
- **Events**: notes such as a ban, a holiday or missing data. They explain dips and jumps on the Dashboard.
- Use the Edit or Delete buttons on a row. Delete always asks first.

---

## Grading

Tracks cards you send to a grading company.

1. Press **Add card**: the card, the company and service, its raw value and the grading cost.
2. Fill in the *sent* date, later the *received* date, the grade and the graded value.
3. The table shows **Win / loss** for each card: graded value minus raw value minus grading cost.
4. The grading fee itself is an expense. Enter it under *Finance, Expenses* (category Grading); this screen does not count it a second time.

---

## eBay plan

A plan for building up your eBay sales.

- At the top you see your goal (number of eBay sales by a date) and how many stock lines are marked as listed on eBay.
- Pick a tab: **Live on eBay now**, **Fast sales**, **Middle** or **Premium**, or **All**. Each card shows a suggested price, what you keep after fee and postage, and a link to what it sold for on eBay.
- Type the sold price you find as a comparison and press **Save**; the suggested price then follows it.
- To update the list of live listings, open *Update from eBay*, paste your Active listings and press the button. Prices are suggestions: you stay in control.

---

## Settings

| Tab | What you set |
|---|---|
| Fees | Cardmarket, eBay and Vinted fee % and fixed amounts, where you verified them, a "confirmed" tick; shipping on every order; the optional eBay shipping adjustment (starts at €0) |
| eBay | Your eBay site and, only if you want automatic eBay orders and the List on eBay button, your eBay developer keys (connect once; eBay asks you to approve reading orders and managing listings; TCGPro creates a listing only when you press List on eBay; with that permission it also keeps your eBay quantities equal to your stock by itself). This is advanced and optional: eBay may ask for extra approval before it gives out production keys, and if that happens you can skip it and type eBay sales by hand |
| Reference data | The card reference pack and its update |
| Pricing | Pricing strategies (% of reference per marketplace, undercut lowest listing, rounding, minimum price); rules per game and/or price range; condition factors |
| Price data & catalog | Download status per game and *Refresh*; when prices count as stale or volatile; improving the catalog from a Cardmarket stock export; linking manual cards |
| Acquisitions & aging | Which purchase fields are required, optional or hidden; slow-moving threshold and price-cut steps |
| Backup & restore | Back up now, external drive, automatic backups, restore, data check |
| Security & devices | Network access and the address for other devices; change password; stop the app |
| Activity log | Every change to stock, costs, prices, sales and settings |
| About | Your subscription (plan, renewal, cancel, licence key), version, this user guide, licence, third-party notices, your data folder, colour theme |

Strategy choice works in this order:
1. A strategy set on a card always wins.
2. Otherwise, the highest-priority matching rule applies. For example: "One Piece cards with a reference of €20 or more → *Premium*".
3. If no rule matches, the default strategy is used.

---

## Contact

Questions, a problem, or something that does not work? Use the contact form at https://mytcgpro.com/pages/contact. Tell us your TCGPro version (Settings, About) and what you see on screen. Please never send your password or your recovery key: we will never ask for them.
