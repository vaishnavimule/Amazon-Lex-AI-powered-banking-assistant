# 💬 Step 3 – Testing the Banking Bot

Once your intents and Lambda integration are ready, test your chatbot directly in the **Amazon Lex Console**.

---

## 🧩 Testing Process

1. Open **Amazon Lex → Test Bot Window**
2. Enter sample inputs like:
   - “What’s my balance?”
   - “Transfer $300 to savings”
   - “Show my mini statement”

---

### 🖼️ Chat Demo

![Chat Demo](screenshots/chat-demo.png)

---

## ✅ Expected Behavior

| User Input | Bot Response |
|-------------|--------------|
| “What’s my balance?” | “Your current balance is $2,450.00.” |
| “Transfer $300 to savings” | “Transfer successful! New balance is $2,150.00.” |
| “Mini statement” | “Here are your last 5 transactions…” |

---

### 💡 Tips
- Use **session attributes** to maintain state between turns.
- Validate slot inputs using Lambda before proceeding.
