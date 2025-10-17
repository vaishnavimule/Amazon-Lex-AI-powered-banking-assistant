# 📊 Step 4 – CloudWatch Monitoring

Monitoring and debugging are crucial to ensure the chatbot runs smoothly.

---

## 🧩 Overview

Every Lex-to-Lambda interaction generates logs in **Amazon CloudWatch**, which helps analyze performance, latency, and errors.

---

### 🖼️ Example CloudWatch Log

![CloudWatch Logs](screenshots/cloudwatch-logs.png)

---

## 🔍 How to Debug
1. Go to **AWS Console → CloudWatch → Log Groups**
2. Select your **Lambda function name**
3. Open latest log stream
4. Check:
   - Event payloads
   - Slot values
   - Response structure
   - Any `KeyError` or `TypeError` messages

---

## 📈 Benefits of Monitoring
- Validate if intents and slots are working as expected
- Detect input mismatches early
- Measure response times and optimize Lambda logic
