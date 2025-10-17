
# 🤖 AWS Lex Conversational AI Projects

This repository demonstrates a complete end-to-end **Conversational AI system** built using **Amazon Lex**, **AWS Lambda (Python)**, **DynamoDB**, **API Gateway**, and **Amazon Translate**.

---

## 🌐 Overview
The project covers the design, configuration, and deployment of multiple AI-driven chatbots capable of handling different intents and integrations.

---

## 🧩 Architecture & Flow

### Architecture Diagram
![Architecture Diagram]![1293e713-9775-4dae-8425-b83646792475](https://github.com/user-attachments/assets/605ea245-9918-4553-beea-5326da54f8f9)


1. **User Input:** The user interacts with the chatbot through the Lex interface.
2. **Amazon Lex:** Detects the intent, extracts slots, and triggers Lambda.
3. **AWS Lambda (Python):** Executes fulfillment logic and retrieves data.
4. **Integrations:** Connects with DynamoDB, API Gateway, or Translate.
5. **Response:** Returns structured reply to the user.

---

## 🐍 Lambda Function

```python
def lambda_handler(event, context):
    intent = event['currentIntent']['name']
    if intent == 'OrderStatus':
        return check_order_status(event)
    elif intent == 'GreetingIntent':
        return {
            "dialogAction": {
                "type": "Close",
                "fulfillmentState": "Fulfilled",
                "message": {"contentType": "PlainText", "content": "Hello! How can I assist you today?"}
            }
        }
```

---

## 💡 Flow with Screenshots

### Step 1: Define Intents
![Lex Intents](screenshots/lex-intents.png)

### Step 2: Lambda Integration
![Lambda Function](screenshots/lambda-code.png)

### Step 3: Testing in Lex Console
![Chat Demo](screenshots/chat-demo.png)

### Step 4: Monitoring with CloudWatch
![CloudWatch Logs](screenshots/cloudwatch-logs.png)

---

## 🧠 Skills Demonstrated

- Conversational AI Development
- AWS Lex, Lambda, DynamoDB, API Gateway, Translate
- Serverless architecture design
- Python scripting for backend fulfillment
- Real-time monitoring and debugging

---

## 👩‍💻 Author
**Vaishnavi Mule**  
Data & AI Analyst | AWS Conversational AI Developer | Snowflake Certified  
📍 Chicago, IL  
🔗 [LinkedIn](https://linkedin.com/in/vaishnavimule) • [GitHub](https://github.com/vaishnavimule)
