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

# 持分法の基本モデル（親会社＋関連会社）

このPythonスクリプトは、親会社が関連会社に出資している場合の**基本的な持分法の会計モデル**を示しています。  
親会社が関連会社の利益をどのように認識し、配当金を処理し、貸借対照表に反映させるかをシミュレーションします。

---

## 📌 概要

持分法は、企業が他社に**重要な影響力**を持つ場合（通常20〜50％の出資比率）に用いられる会計手法です。  

この方法では：

1. 親会社は関連会社の純利益の持分を投資勘定に加算します。  
2. 関連会社から受け取った配当金は投資勘定を減額します。  
3. 親会社の貸借対照表には、**関連会社の個別資産・負債ではなく、調整後の投資額**が反映されます。

本スクリプトでは、以下の単純なケースをモデル化しています：

- 親会社：1社  
- 関連会社：1社  
- 出資比率：40％  
- 例として純利益・配当金を設定  

---

## 🛠 必要環境

- Python 3.x  
- `pandas` ライブラリ  

pandasが未インストールの場合は以下でインストール可能です：

```bash
pip install pandas
⚙️ 使い方
Python環境でスクリプトを開きます。

必要に応じて初期データを変更します：

python
コードをコピーする
ownership = 0.4  # 親会社の出資比率
parent_investment = 1000  # 関連会社への初期投資額
associate_net_income = 500  # 関連会社の純利益
dividend_paid = 100  # 関連会社からの配当金
スクリプトを実行します。

以下の情報が出力されます：

持分利益反映後の親会社投資勘定

配当金処理後の投資勘定

持分法適用後の親会社貸借対照表

処理のステップごとの説明

📊 実行例
yaml
コードをコピーする
親会社の投資勘定（持分利益反映後）: 1200.0
配当金処理後の投資勘定: 1160.0

親会社の貸借対照表（持分法適用後）:
                                   現金  関連会社株式（投資勘定）  純資産合計
親会社（持分法適用後）                540                    1160         1700

【処理の流れ】
① 関連会社の純利益500のうち40%（200）を親会社の投資勘定に加算。
② 関連会社からの配当金100のうち40%（40）を受け取り、投資勘定を40減額。
③ 結果として投資勘定は +160増加（1000→1160）。
📈 処理の仕組み
持分利益の認識
親会社は関連会社の純利益の持分を投資勘定に加算します：

持分利益
=
関連会社の純利益
×
出資比率
持分利益=関連会社の純利益×出資比率
配当金の処理
親会社が配当金を受け取ると、投資勘定は親会社持分分だけ減額されます：

投資勘定の減少額
=
配当金
×
出資比率
投資勘定の減少額=配当金×出資比率
貸借対照表への反映
親会社の貸借対照表には以下が反映されます：

現金（配当金受取分を含む）

関連会社株式（投資勘定）（持分利益・配当金反映後）

純資産合計 = 現金 + 投資勘定

📜 ライセンス
このスクリプトは教育目的で使用可能です。
持分法の理解のために自由に修正・利用できます。
