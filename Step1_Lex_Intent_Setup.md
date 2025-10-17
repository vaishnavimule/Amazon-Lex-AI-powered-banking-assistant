# 🧠 Step 1 – Amazon Lex Intent Setup

This step focuses on configuring **Amazon Lex** for the banking assistant.

---

## 🧩 Overview
Amazon Lex is used to design conversational flow through **intents**, **utterances**, and **slots**.

### 🏦 Example Intents:
| Intent | Description |
|--------|--------------|
| `CheckBalance` | Fetches the user's current account balance |
| `FundTransfer` | Transfers funds between accounts |
| `MiniStatement` | Displays last 5 transactions |
| `GreetingIntent` | Handles basic greetings |
| `HelpIntent` | Provides bot usage guidance |

---

## 🖼️ Lex Console Setup

![Lex Intents](screenshots/lex-intents.png)

- Define **intents** with sample utterances like:
  - “Check my balance”
  - “Transfer $500 to savings”
  - “Show my mini statement”

- Create **slots** to capture dynamic data such as:
  - `accountNumber`
  - `amount`
  - `targetAccount`
  - `pin`

---

Once the intents are ready, connect each to your **Lambda function ARN** for fulfillment.
