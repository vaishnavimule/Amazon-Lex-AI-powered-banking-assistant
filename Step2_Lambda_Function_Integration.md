# ⚙️ Step 2 – AWS Lambda Function Integration

This step shows how to integrate **Amazon Lex** with **AWS Lambda** for backend fulfillment.

---

## 🧩 Overview

The **BankingBotEnglish.py** file contains all logic for routing intents, performing calculations, and generating responses.

### 🐍 Core Lambda Structure:

```python
def lambda_handler(event, context):
    intent = event['currentIntent']['name']
    
    if intent == 'CheckBalance':
        return get_balance(event)
    elif intent == 'FundTransfer':
        return transfer_funds(event)
    elif intent == 'MiniStatement':
        return get_mini_statement(event)
```

---

## 🖼️ Lambda Function Console

![Lambda Function](screenshots/lambda-code.png)

- Runtime: **Python 3.9**
- Environment: AWS Lambda Console  
- Connected to Amazon Lex as a fulfillment function  
- Logs output to **Amazon CloudWatch**  

---

### 🧠 Logic Summary

| Function | Description |
|-----------|--------------|
| `get_balance()` | Fetches user balance from DynamoDB |
| `transfer_funds()` | Validates accounts and processes transaction |
| `get_mini_statement()` | Retrieves latest transactions |
| `verify_user()` | Confirms account and PIN |
