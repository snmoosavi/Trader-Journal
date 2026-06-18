# Trading Journal — Complete User Guide

**Trading Journal** is a Windows desktop application designed to help traders plan trades, control risk, journal executions, review performance, and build a more disciplined trading process.

The app is built around one main idea:

> Better trading starts with better process control.

Trading Journal is not a broker, not an exchange, not an automated trading robot, and not a signal service. It is a local-first journaling and decision-review tool that helps you document what you planned, what you did, what happened, and what you can improve.

---

## Table of Contents

1. [What Trading Journal Is](#what-trading-journal-is)
2. [What Trading Journal Is Not](#what-trading-journal-is-not)
3. [Core Workflow](#core-workflow)
4. [Main App Sections](#main-app-sections)
5. [Session Tab](#session-tab)
6. [Pre-Trade Gate](#pre-trade-gate)
7. [Risk-Based Position Sizing](#risk-based-position-sizing)
8. [Guardrails](#guardrails)
9. [Journal Tab](#journal-tab)
10. [Adding a Trade Manually](#adding-a-trade-manually)
11. [Editing and Deleting Trades](#editing-and-deleting-trades)
12. [Trade Screenshots](#trade-screenshots)
13. [CSV Import](#csv-import)
14. [CSV Export](#csv-export)
15. [Reports Tab](#reports-tab)
16. [Setup Score Tab](#setup-score-tab)
17. [Price Charts Tab](#price-charts-tab)
18. [Mini Panel / HUD](#mini-panel--hud)
19. [Settings Tab](#settings-tab)
20. [System Tray Behavior](#system-tray-behavior)
21. [Micro and Mini Futures Contracts](#micro-and-mini-futures-contracts)
22. [Local Data Storage](#local-data-storage)
23. [Backup and Restore](#backup-and-restore)
24. [Recommended Daily Routine](#recommended-daily-routine)
25. [Example Trading Workflows](#example-trading-workflows)
26. [CSV Examples](#csv-examples)
27. [Performance Metrics Explained](#performance-metrics-explained)
28. [Troubleshooting](#troubleshooting)
29. [Frequently Asked Questions](#frequently-asked-questions)
30. [Privacy and Safety](#privacy-and-safety)
31. [Important Disclaimer](#important-disclaimer)
32. [Support](#support)

---

## What Trading Journal Is

Trading Journal is a desktop trading companion for Windows. It helps traders create a structured routine before, during, and after trading.

The app is focused on:

- Trade planning
- Pre-trade checklist discipline
- Risk calculation
- Daily trading limits
- Journaling trade details
- Recording emotions and notes
- Attaching chart screenshots
- Importing trades from CSV files
- Exporting journal records
- Reviewing performance reports
- Tracking win rate, profit factor, expectancy, drawdown, and equity curve
- Scoring trade setup quality
- Keeping trading data stored locally on your own device

Trading Journal is designed for traders who want to improve their process instead of only focusing on individual wins or losses.

---

## What Trading Journal Is Not

Trading Journal is not a trading platform.

It does **not**:

- Place trades
- Connect directly to your broker
- Automatically execute orders
- Automatically pull broker account data
- Provide buy or sell signals
- Predict market direction
- Guarantee profits
- Replace a trading plan
- Replace risk management
- Provide financial advice

The app is a journaling, planning, risk-awareness, and review tool. You remain responsible for your own trading decisions.

---

## Core Workflow

A simple Trading Journal workflow looks like this:

1. Start your trading session.
2. Review your rules using the Pre-Trade Gate.
3. Calculate position size before entering a trade.
4. Check guardrails such as daily loss limit and max trades per day.
5. Take only planned trades.
6. Record every completed trade in the Journal.
7. Add screenshots and notes.
8. Review your performance in Reports.
9. Export or back up your data regularly.
10. Improve your rules based on repeated patterns.

The app is most useful when used consistently. The goal is to create a repeatable trading review habit.

---

## Main App Sections

Trading Journal includes the following main sections:

### Session

The Session tab gives you a daily overview, checklist, risk calculator, and guardrail status.

### Journal

The Journal tab is where you add, edit, delete, import, export, and review trade records.

### Reports

The Reports tab shows performance metrics and an equity curve based on saved trades.

### Price Charts

The Price Charts tab can display USD price charts using public market data where available.

### Setup Score

The Setup Score tab evaluates a trade idea and produces a setup score from 0 to 100.

### Settings

The Settings tab lets you configure appearance, risk defaults, guardrails, checklist items, mini panel behavior, tray behavior, and data options.

---

## Session Tab

The Session tab is designed to help you stay aware of your current trading day.

It may show:

- Trades today
- PnL today
- Consecutive losses
- Guardrail status
- Pre-trade checklist
- Risk calculator
- Session start/stop controls

Use this tab before and during trading.

### Why the Session Tab Matters

Many trading mistakes happen before the trade is even entered:

- Entering without a setup
- Risking too much
- Trading after a loss streak
- Trading without checking news
- Revenge trading
- Overtrading
- Ignoring daily loss limits

The Session tab helps reduce these mistakes by putting your rules in front of you.

---

## Pre-Trade Gate

The Pre-Trade Gate is a structured checklist that helps you confirm whether a trade follows your rules before entering.

Typical checklist items include:

- The setup is clearly defined.
- Entry, stop, and target are valid.
- Risk is within the allowed limit.
- Major news or events have been checked.
- You are not revenge trading.
- The invalidation plan is clear.
- You know when and why you will exit.

### How to Use the Pre-Trade Gate

1. Go to the Session tab.
2. Read each checklist item.
3. Check each item only if it is truly satisfied.
4. If important items are not satisfied, do not force the trade.
5. Use the checklist as a discipline filter, not as a formality.

### Best Practice

Do not make checklist items too vague.

Weak checklist item:

> Looks good.

Better checklist item:

> Entry, stop, and target are defined before entering.

Better checklist items create better review data.

---

## Risk-Based Position Sizing

The risk calculator helps estimate position size based on your account and trade risk.

It uses values such as:

- Account equity
- Risk percentage
- Entry price
- Stop price
- Quantity step

### Basic Formula

The general logic is:

```text
Risk Amount = Account Equity × Risk Percentage
Stop Distance = Absolute difference between Entry and Stop
Suggested Quantity = Risk Amount ÷ Stop Distance
```

Example:

```text
Account Equity: 10,000
Risk Percentage: 1%
Entry: 100
Stop: 98

Risk Amount = 10,000 × 1% = 100
Stop Distance = 100 - 98 = 2
Suggested Quantity = 100 ÷ 2 = 50
```

This means the suggested quantity is 50 units if each point of movement equals 1 unit of currency.

### Important Note for Futures

For futures contracts, risk often depends on tick size, tick value, and point value. The app’s standard risk calculator is a general position sizing tool. Futures traders should always confirm contract-specific values using their broker or exchange specifications.

---

## Guardrails

Guardrails help prevent emotional or excessive trading.

Trading Journal includes practical guardrails such as:

- Daily loss limit
- Maximum trades per day
- Cooldown after consecutive losses

These features are not meant to control the market. They are meant to control trader behavior.

---

### Daily Loss Limit

The daily loss limit helps you define the maximum amount you are willing to lose in a day.

Example:

```text
Daily Loss Limit: 300
```

If your PnL today reaches or passes this loss level, the app can show that guardrails are limited or triggered.

### Why It Matters

A daily loss limit helps prevent one bad day from becoming a catastrophic day.

---

### Maximum Trades Per Day

This setting helps reduce overtrading.

Example:

```text
Maximum Trades Per Day: 5
```

After reaching the limit, the app can warn that trading should be limited.

### Why It Matters

More trades do not always mean better performance. Many traders perform worse after taking too many trades.

---

### Consecutive Loss Cooldown

This guardrail helps reduce revenge trading.

Example:

```text
Maximum Consecutive Losses: 3
Cooldown: 30 minutes
```

If you take three losing trades in a row, the app can indicate that a cooldown is active.

### Why It Matters

A losing streak often increases emotional pressure. A cooldown creates space before the next decision.

---

## Journal Tab

The Journal tab is the main record-keeping area.

Use it to:

- View saved trades
- Filter trades by date
- Add trades manually
- Edit trades
- Delete trades
- Import trades from CSV
- Export trades to CSV

The journal table includes key fields such as:

- Date
- Symbol
- Side
- Entry
- Stop
- Target
- Quantity
- PnL
- R-multiple
- Setup
- Setup score

---

## Adding a Trade Manually

To add a trade:

1. Open the Journal tab.
2. Click **Add Trade**.
3. Fill in the trade details.
4. Add notes or emotions if useful.
5. Attach before/after screenshots if needed.
6. Save the trade.

### Trade Fields Explained

#### Date

The date of the trade.

#### Symbol

The instrument or market traded.

Examples:

```text
AAPL
BTC-USD
EURUSD
MES
MNQ
ES
NQ
```

#### Side

The trade direction:

- LONG
- SHORT

#### Entry

The entry price.

#### Stop

The stop loss price.

#### Target

The planned target price.

#### Quantity

The position size or number of contracts/shares/units.

#### PnL

Profit or loss for the trade.

Positive number = winning trade  
Negative number = losing trade

#### R-Multiple

R-multiple describes the result relative to the original risk.

Example:

```text
+2R = profit was two times the planned risk
-1R = full planned risk was lost
```

#### Setup / Tag

A label for the trade type.

Examples:

```text
Breakout
Pullback
Reversal
Opening Range
Trend Continuation
Scalping
News Trade
```

#### Emotions

A short description of your emotional state.

Examples:

```text
Calm
Confident
Rushed
Fearful
Greedy
Revenge trading
Patient
```

#### Notes

Use notes to record:

- Trade thesis
- Why you entered
- What you expected
- What actually happened
- Mistakes
- Lessons
- Management decisions
- Rule violations

Good notes are one of the most valuable parts of a trading journal.

---

## Editing and Deleting Trades

### Editing a Trade

To edit a trade:

1. Go to the Journal tab.
2. Select the trade.
3. Click **Edit** or double-click the row.
4. Update the fields.
5. Save changes.

### Deleting a Trade

To delete a trade:

1. Select the trade in the Journal tab.
2. Click **Delete**.
3. Confirm the deletion.

Use delete carefully. If you want to preserve an audit trail, consider editing notes instead of deleting.

---

## Trade Screenshots

Trading Journal allows before and after screenshots for each trade.

### Before Screenshot

A before screenshot is useful for capturing:

- Market structure
- Setup context
- Entry zone
- Stop placement
- Target area
- Pre-trade plan

### After Screenshot

An after screenshot is useful for reviewing:

- Whether the trade followed the plan
- How price reacted
- Whether exit management was good
- Whether the stop or target placement was reasonable
- Whether emotions affected decisions

### Best Practice

Attach screenshots to your most important trades, losing trades, and rule-breaking trades. These often provide the most learning value.

---

## CSV Import

Trading Journal includes a professional CSV import workflow.

Use CSV import when you already have trade data exported from another platform, spreadsheet, or broker report.

The import system supports:

- Selecting a CSV file
- Reading common CSV formats
- Flexible column mapping
- Previewing rows before import
- Detecting invalid rows
- Detecting duplicate trades
- Importing only ready rows
- Showing an import summary

---

### How to Import a CSV File

1. Open the Journal tab.
2. Click **Import CSV...**
3. Select your CSV file.
4. Review the column mapping.
5. Check the preview table.
6. Fix mappings if required.
7. Click **Import Ready Rows**.
8. Review the import summary.

You can also use the menu:

```text
File → Import CSV to Journal...
```

Shortcut:

```text
Ctrl + I
```

---

### CSV Column Mapping

Different brokers and platforms use different column names.

For example, one file may use:

```text
Symbol, Side, Quantity, Net P/L
```

Another file may use:

```text
Instrument, Direction, Qty, RealizedPnL
```

Trading Journal allows you to map each CSV column to the correct journal field.

---

### Supported Import Fields

The importer can map common fields such as:

- Date
- Symbol
- Side / Direction
- Entry
- Stop
- Target
- Qty / Quantity
- PnL
- R
- Setup
- Emotions
- Notes
- Trade ID

---

### Required Fields

At minimum, the import process needs enough information to create a valid journal entry.

Recommended required fields:

- Date
- Symbol
- Side / Direction
- Quantity
- PnL

In the app, Date and Symbol are especially important. If Side is missing but Quantity is signed, the app may be able to derive direction from the quantity.

Example:

```text
Qty = 2     → Long
Qty = -2    → Short
```

---

### Preview Table

Before importing, the app shows a preview.

The preview helps you see:

- Rows ready to import
- Rows that will be skipped
- Invalid rows
- Duplicate trades
- Missing required values
- Invalid dates
- Invalid numeric values

Do not skip the preview step. It helps prevent bad data from entering your journal.

---

### Duplicate Detection

The importer tries to avoid importing duplicate trades.

Duplicates may be detected using:

- Trade ID, if available
- Trade date
- Symbol
- Direction
- Entry
- Quantity
- PnL

If a row appears to be a duplicate, it may be skipped.

---

### Import Summary

After import, the app shows a summary:

- Imported rows
- Skipped rows
- Rows with errors

Use this summary to confirm whether the import worked correctly.

---

## CSV Export

CSV export lets you save your journal data outside the app.

Use export to:

- Back up your journal
- Analyze data in Excel
- Move records to another system
- Share data with a coach or mentor
- Keep an external archive

To export:

1. Go to the Journal tab.
2. Apply any date filter if needed.
3. Click **Export CSV**.
4. Choose a file location.
5. Save the file.

### Export Best Practice

Export your journal regularly, especially before:

- Updating the app
- Reinstalling Windows
- Moving to a new PC
- Testing new versions
- Cleaning app folders

---

## Reports Tab

The Reports tab converts your saved trade data into performance metrics.

Reports may include:

- Total trades
- Wins
- Losses
- Win rate
- Total PnL
- Average PnL
- Profit factor
- Expectancy
- Maximum drawdown
- Best trade
- Worst trade
- Equity curve

### How to Use Reports

1. Record trades consistently.
2. Open the Reports tab.
3. Review the summary metrics.
4. Look for repeated strengths and weaknesses.
5. Compare performance by date ranges if available.
6. Use the insights to improve rules and execution.

Reports are only as useful as the data you record. Missing trades or inaccurate PnL values will reduce report quality.

---

## Setup Score Tab

The Setup Score tab helps evaluate trade setup quality.

It produces:

- Score from 0 to 100
- Strength label: Weak, Medium, or Strong
- Setup summary
- Option to copy the summary
- Option to save the scored setup to the Journal

### What the Score Means

A setup score is a process-quality indicator. It can help you evaluate whether a trade idea has enough structure.

Example interpretation:

```text
0–44    Weak
45–69   Medium
70–100  Strong
```

### Important Note

The Setup Score is not a trading signal. A strong setup can still lose. A weak setup can still win. The score is intended to help you review quality and consistency, not predict the market.

---

## Price Charts Tab

The Price Charts tab provides USD price charts using public API data where available.

Depending on the version and availability, the app may load public market products and chart candles for selected ranges.

### Available Ranges May Include

- 1 Day
- 7 Days
- 30 Days
- 90 Days
- 1 Year

### Important Notes

Price Charts:

- Require internet access
- Depend on public API availability
- May be rate-limited
- May not support every symbol
- Are separate from the journal
- Are not a broker feed
- Do not place trades
- Do not provide trading signals

If Price Charts are unavailable, the journal, reports, risk calculator, and local data features can still be used.

---

## Mini Panel / HUD

The Mini Panel is a compact always-available window that helps you monitor your trading state without keeping the full app open.

It may show:

- Session status
- Pre-trade gate status
- Today’s trade count
- Today’s PnL
- Guardrail status
- Current risk amount
- Suggested quantity

The Mini Panel can also provide quick actions such as:

- Open the main app
- Start or stop session
- Add trade
- Hide mini panel

### How to Toggle the Mini Panel

Use:

```text
View → Toggle Mini Panel
```

You can also configure Mini Panel behavior in Settings.

---

## Settings Tab

The Settings tab lets you customize the app.

Available settings may include:

### Appearance

- Dark Mode

### Risk Defaults

- Default account equity
- Default risk percentage
- Default quantity step

### Guardrails

- Daily loss limit
- Maximum trades per day
- Maximum consecutive losses
- Cooldown duration

### Checklist

- Edit pre-trade checklist items

### Mini Panel

- Enable or disable Mini Panel
- Auto-show Mini Panel when minimizing
- Dock Mini Panel to bottom-right

### System Tray

- Enable or disable tray behavior
- Choose close behavior
- Show or hide tray balloon notifications

### Data Tools

- Open data folder
- Backup database
- Restore database

The exact settings available may vary by version.

---

## System Tray Behavior

Trading Journal supports system tray behavior.

This means the app can continue running in the tray instead of fully closing.

### Close Options

When closing the app, you may see options such as:

- Minimize to Tray
- Exit
- Cancel
- Remember my choice

### Useful Shortcuts

Depending on version:

```text
Ctrl + I    Import CSV to Journal
Ctrl + M    Minimize to Tray
Ctrl + Q    Exit
F1          Open Program Guide
```

### Best Practice

If you want Trading Journal available during the trading day, use Minimize to Tray. If you are finished trading, use Exit.

---

## Micro and Mini Futures Contracts

Trading Journal can be used to journal micro and mini futures trades manually or through CSV import.

Examples include:

```text
MES   Micro E-mini S&P 500
MNQ   Micro E-mini Nasdaq
MYM   Micro E-mini Dow
M2K   Micro E-mini Russell 2000
ES    E-mini S&P 500
NQ    E-mini Nasdaq
YM    E-mini Dow
RTY   E-mini Russell 2000
MGC   Micro Gold
MCL   Micro Crude Oil
GC    Gold
CL    Crude Oil
```

### Manual Journaling

You can manually enter futures symbols in the Symbol field.

Example:

```text
Symbol: MES
Side: LONG
Entry: 5400.25
Stop: 5395.25
Qty: 2
PnL: 50
```

### CSV Import for Futures

If your broker or platform exports futures trades to CSV, you can import them through the CSV import tool.

### Automatic Broker Data

Trading Journal does not currently connect directly to brokers or trading platforms to automatically pull futures trade data.

Automatic integration would require platform-specific review because each broker/platform may have different:

- APIs
- Authentication
- Permissions
- Data formats
- Symbol formats
- Commission handling
- Time zone handling
- Partial fill handling
- Rate limits
- Market data rules

For now, use manual entry or CSV import.

---

## Local Data Storage

Trading Journal is local-first.

Your journal is stored on your own device using a local SQLite database.

The app may create a local data folder containing:

```text
data/
  trading_journal.db
  screenshots/
  logs/
```

### What This Means

Your journal data is not automatically uploaded to a cloud server by the app.

You are responsible for:

- Backing up your data
- Protecting your device
- Exporting important records
- Keeping copies before reinstalling or moving computers

---

## Backup and Restore

Backing up your journal is important.

### Recommended Backup Methods

Use one or more of the following:

1. Export CSV regularly.
2. Back up the app data folder.
3. Copy the SQLite database file.
4. Keep screenshots with your journal backups.
5. Store backups in a safe location.

### When to Back Up

Back up before:

- Updating the app
- Reinstalling Windows
- Moving to another computer
- Testing a new version
- Deleting old data
- Restoring from another file

### Restore Warning

Restoring a database may replace current data. Always create a backup before restoring.

---

## Recommended Daily Routine

Here is a recommended daily workflow.

### Before Market Open

1. Open Trading Journal.
2. Review previous trading mistakes.
3. Set or confirm guardrails.
4. Check the Pre-Trade Gate.
5. Confirm daily loss limit.
6. Confirm max trades per day.
7. Prepare symbols or markets to watch.

### Before Each Trade

1. Confirm the setup.
2. Check entry, stop, and target.
3. Calculate position size.
4. Confirm risk is acceptable.
5. Check whether guardrails are still OK.
6. Take a screenshot if useful.
7. Enter only if the trade follows your plan.

### After Each Trade

1. Add the trade to the Journal.
2. Record PnL and R-multiple.
3. Add notes.
4. Record emotions.
5. Attach an after screenshot if useful.
6. Mark whether the trade followed your rules.

### End of Day

1. Review Reports.
2. Review losing trades.
3. Review rule-breaking trades.
4. Export CSV if needed.
5. Write one improvement for tomorrow.

---

## Example Trading Workflows

### Workflow 1: Manual Day Trader

1. Start session.
2. Use Pre-Trade Gate.
3. Calculate risk.
4. Take trade in your broker platform.
5. Add trade manually after exit.
6. Attach chart screenshot.
7. Review end-of-day performance.

### Workflow 2: Futures Trader Using CSV

1. Trade through your futures platform.
2. Export fills or closed trades to CSV.
3. Open Trading Journal.
4. Click Import CSV.
5. Map columns.
6. Preview rows.
7. Import ready rows.
8. Review Reports.

### Workflow 3: Review-Focused Trader

1. Import or manually enter trades.
2. Tag each trade by setup type.
3. Add emotions and notes.
4. Review win rate and expectancy.
5. Identify which setup tags perform best.
6. Update your trading plan.

---

## CSV Examples

### Simple CSV Example

```csv
Date,Symbol,Side,Entry,Stop,Target,Qty,PnL,Setup,Notes
2026-06-18,MES,LONG,5400.25,5395.25,5410.25,2,100,Pullback,Followed plan
2026-06-18,MNQ,SHORT,19500.50,19530.50,19440.50,1,-60,Breakdown,Exited at stop
```

### CSV With Alternative Column Names

```csv
TradeDate,Instrument,Direction,AveragePrice,Quantity,NetPnL,Strategy,Comment
2026-06-18,ES,BUY,5400.25,1,125,Opening Range,Good execution
2026-06-18,NQ,SELL,19500.50,-1,-80,Reversal,Entered too early
```

In the import mapping screen, you can map:

```text
TradeDate      → Date
Instrument     → Symbol
Direction      → Side / Direction
AveragePrice   → Entry
Quantity       → Qty
NetPnL         → PnL
Strategy       → Setup
Comment        → Notes
```

### Common Import Problems

#### Problem: Date not recognized

Try a standard date format:

```text
YYYY-MM-DD
```

Example:

```text
2026-06-18
```

#### Problem: PnL contains currency symbols

The importer may handle many numeric formats, but clean numbers are best.

Better:

```text
125.50
```

Instead of:

```text
$125.50 USD
```

#### Problem: Side is missing

Add a Side column with:

```text
LONG
SHORT
BUY
SELL
```

Or use signed quantity if supported:

```text
2     = Long
-2    = Short
```

---

## Performance Metrics Explained

### Total Trades

The number of trades in the selected report range.

### Wins

Trades with positive PnL.

### Losses

Trades with negative PnL.

### Win Rate

Percentage of trades that were profitable.

Formula:

```text
Win Rate = Winning Trades ÷ Total Trades × 100
```

### Total PnL

The sum of all trade profits and losses.

### Average PnL

Average result per trade.

Formula:

```text
Average PnL = Total PnL ÷ Number of Trades
```

### Profit Factor

Profit Factor compares gross profit to gross loss.

Formula:

```text
Profit Factor = Gross Profit ÷ Absolute Gross Loss
```

Example:

```text
Gross Profit: 2,000
Gross Loss: 1,000
Profit Factor: 2.0
```

A profit factor above 1 means gross profits are greater than gross losses.

### Expectancy

Expectancy is the average amount you expect to make or lose per trade based on your historical results.

Simple formula used in many journals:

```text
Expectancy = Total PnL ÷ Number of Trades
```

### Maximum Drawdown

Maximum drawdown shows the largest peak-to-trough decline in the equity curve.

It helps measure how much your account or strategy declined before recovering.

### Best Trade

The highest PnL trade.

### Worst Trade

The lowest PnL trade.

### Equity Curve

The equity curve shows cumulative PnL over time.

It helps you see:

- Growth periods
- Drawdowns
- Volatility
- Consistency
- Performance changes

---

## Troubleshooting

### The App Does Not Open

Try:

1. Restart Windows.
2. Run the app again.
3. Check whether antivirus software blocked it.
4. Reinstall the app.
5. Make sure Windows is updated.
6. Contact support with a screenshot or error message.

---

### My Data Is Missing

Possible reasons:

- You are running the app from a different folder.
- The data folder changed.
- The database file was moved or deleted.
- You restored an older database.
- You are using a different Windows user account.

Recommended actions:

1. Open the app data folder from Settings if available.
2. Look for `trading_journal.db`.
3. Check whether you have a backup.
4. Check exported CSV files.

---

### CSV Import Fails

Check:

- The CSV has a header row.
- Date column is mapped.
- Symbol column is mapped.
- Number fields contain valid numbers.
- The file is not open in Excel.
- The file is saved as CSV, not XLSX.
- The file is not empty.
- The delimiter is common, such as comma, semicolon, tab, or pipe.

---

### CSV Rows Are Skipped

Rows may be skipped because:

- Date is missing.
- Symbol is missing.
- Date format is invalid.
- Side cannot be detected.
- Numeric fields are invalid.
- The row appears to be a duplicate.

Review the preview table and error column before importing.

---

### Reports Look Wrong

Check:

- PnL values are entered correctly.
- Losses are negative numbers.
- Wins are positive numbers.
- Date filters are correct.
- Duplicate trades were not imported.
- All trades are recorded.
- Imported trades were mapped correctly.

---

### Price Charts Do Not Load

Possible reasons:

- No internet connection
- Public API is unavailable
- API rate limit
- Product is not supported
- Temporary network error
- Missing dependency in a development build

The rest of the app can still be used without charts.

---

### Mini Panel Is Not Visible

Try:

1. Go to View.
2. Select Toggle Mini Panel.
3. Check Settings to make sure Mini Panel is enabled.
4. If it is docked off-screen, restart the app.

---

### The App Minimizes Instead of Closing

The close behavior may be set to minimize to tray.

Check:

```text
Settings → System Tray / Close Behavior
```

Or use:

```text
File → Exit
```

Shortcut:

```text
Ctrl + Q
```

---

## Frequently Asked Questions

### Does Trading Journal connect to my broker?

No. Trading Journal does not currently connect directly to brokers.

You can manually enter trades or import CSV files if your broker/platform provides CSV export.

---

### Does the app automatically pull micro or mini futures trades?

No. The app does not automatically pull futures trades from a broker.

You can journal micro and mini futures manually or import them through CSV.

---

### Can I use this for stocks?

Yes. You can manually enter stock symbols and trades.

---

### Can I use this for crypto?

Yes. You can journal crypto trades manually. Price charts may support some USD crypto products where public data is available.

---

### Can I use this for forex?

Yes. You can manually journal forex trades. Use your own symbol format consistently.

---

### Can I import CSV from any broker?

The app supports flexible column mapping, but every broker has different export formats. Most standard CSV exports can be imported if they include usable trade fields.

If a CSV file does not import correctly, check column mapping and field formats.

---

### Does the app store my data online?

No. The app is local-first and stores journal data on your device.

---

### Is this financial advice?

No. Trading Journal is a journaling and review tool. It does not provide financial advice.

---

### Can the app guarantee profitability?

No. No journal can guarantee profits. The app helps you improve process discipline and review quality.

---

### What should I back up?

Back up:

- CSV exports
- `trading_journal.db`
- screenshots folder
- any notes or external files you use with your journal

---

## Privacy and Safety

Trading Journal is designed to keep your journal data local.

The app does not require a broker login to function.

Because data is local, you should:

- Protect your Windows account
- Keep backups
- Avoid sharing your database publicly
- Be careful when sharing screenshots
- Remove sensitive information before sending support files

---

## Important Disclaimer

Trading involves risk.

Trading Journal is provided as a journaling, planning, risk-awareness, and performance-review tool only.

It does not provide financial, investment, tax, legal, or trading advice.

It does not guarantee profits or prevent losses.

It does not place trades.

It does not connect to your broker.

It does not generate trading signals.

You are fully responsible for your own trading decisions, risk management, and compliance with applicable rules and regulations.

---

## Support

For support, questions, feedback, or feature requests, contact:

**sn.moosavi@gmail.com**

When contacting support, please include:

- App name: Trading Journal
- Windows version
- App version if available
- Description of the issue
- Screenshot if possible
- CSV sample if the question is about import
- Steps to reproduce the issue

Please avoid sending sensitive account information, broker passwords, API keys, or private financial details.

---

## Suggested Feedback Format

If you want to request a feature, use this format:

```text
Feature request:
Why I need it:
Example workflow:
CSV sample or screenshot:
Expected result:
```

If you want to report a bug, use this format:

```text
Issue:
Steps to reproduce:
Expected result:
Actual result:
Screenshot:
Windows version:
App version:
```

---

## Final Notes

Trading Journal works best when used consistently.

The most valuable journal is not the one with the most features.  
It is the one you actually use after every trade.

Record your plan.  
Record your execution.  
Record your emotions.  
Review your mistakes.  
Improve one rule at a time.
