# Basic Equity Method Model (Parent Company + Associate)

This Python script demonstrates a **basic equity method accounting model** for a parent company that holds a stake in an associate. It simulates how the parent recognizes its share of the associate’s profit, handles dividends, and reflects these changes in the balance sheet.

---

## 📌 Overview

The equity method is an accounting technique used when a company has **significant influence** over another company (usually 20–50% ownership). Under this method:

1. The parent company recognizes its share of the associate’s net income as an increase in the investment account.
2. Dividends received from the associate reduce the investment account.
3. The parent’s balance sheet reflects the adjusted investment value, **not the associate’s individual assets and liabilities**.

This script models a simple case with:

- 1 parent company  
- 1 associate company  
- Ownership ratio: 40%  
- Example net income and dividend values  

---

## 🛠 Requirements

- Python 3.x  
- `pandas` library  

Install pandas if you don’t have it:

```bash
pip install pandas
⚙️ How to Use
Open the script in a Python environment.

Modify the initial data if needed:

python
コードをコピーする
ownership = 0.4  # Parent's ownership percentage
parent_investment = 1000  # Initial investment in associate
associate_net_income = 500  # Associate's net income
dividend_paid = 100  # Dividend paid by the associate
Run the script.

The output will display:

Parent's investment account after recognizing equity income

Investment account after dividend adjustment

Parent’s balance sheet after equity method application

Step-by-step explanation of the process

📊 Example Output
pgsql
コードをコピーする
Parent company's investment account (after recognizing equity income): 1200.0
Investment account after dividend adjustment: 1160.0

Parent Company's Balance Sheet (After Equity Method):
                                   Cash  Investment in Associate  Total Equity
Parent Company (After Equity Method)  540                    1160         1700

【Process Summary】
① Add 40% (200) of associate's net income 500 to the parent's investment account.
② Receive 40% (40) of dividends 100 from the associate and reduce investment account by 40.
③ Result: Investment account increases by +160 (1000 → 1160).
📈 How It Works
Recognize Equity Income
The parent adds its share of the associate’s net income to the investment account:

Equity Income
=
Associate Net Income
×
Ownership
Equity Income=Associate Net Income×Ownership
Dividend Adjustment
When the parent receives dividends, the investment account decreases by the parent’s share:

Investment Account Reduction
=
Dividends Paid
×
Ownership
Investment Account Reduction=Dividends Paid×Ownership
Balance Sheet Representation
The parent’s balance sheet reflects:

Cash (including dividends received)

Investment in Associate (adjusted for equity income and dividends)

Total Equity = Cash + Investment

📜 License
This script is open for educational purposes. Feel free to modify and use it to learn about the equity method of accounting.
