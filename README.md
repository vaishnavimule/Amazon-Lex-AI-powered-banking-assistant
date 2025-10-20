
# 🤖 Amazon Lex Conversational AI Projects

This repository demonstrates a complete end-to-end **Conversational AI system** built using **Amazon Lex**, **AWS Lambda (Python)**, **DynamoDB**, **API Gateway**, and **Amazon Translate**.

---

## 🌐 Overview
A fully functioning AI chatbot that can:

- Greet users and understand different ways people ask for help
- Recognize specific banking terms and account types
- Retrieve account balances using backend logic
- Remember user information to create smoother conversations

---

## 🧩 Architecture & Flow


![1293e713-9775-4dae-8425-b83646792475](https://github.com/user-attachments/assets/605ea245-9918-4553-beea-5326da54f8f9)


1. **User Input:** The user interacts with the chatbot through the Lex interface.
2. **Amazon Lex:** Detects the intent, extracts slots, and triggers Lambda.
3. **AWS Lambda (Python):** Executes fulfillment logic and retrieves data.
4. **Integrations:** Connects with DynamoDB, API Gateway, or Translate.
5. **Response:** Returns structured reply to the user.

---

## 🐍 Lambda Function

```python
def CheckBalance(intent_request):
    session_attributes = get_session_attributes(intent_request)
    slots = get_slots(intent_request)
    account = get_slot(intent_request, 'accountType')
    #The account balance in this case is a random number
    #Here is where you could query a system to get this information
    balance = str(random_num())
    text = "Thank you. The balance on your "+account+" account is $"+balance+" dollars."
    message =  {
            'contentType': 'PlainText',
            'content': text
        }
    fulfillment_state = "Fulfilled"    
    return close(intent_request, session_attributes, fulfillment_state, message)   

def FollowupCheckBalance(intent_request):
    session_attributes = get_session_attributes(intent_request)
    slots = get_slots(intent_request)
    account = get_slot(intent_request, 'accountType')
    #The account balance in this case is a random number
    #Here is where you could query a system to get this information
    balance = str(random_num())
    text = "Thank you. The balance on your "+account+" account is $"+balance+" dollars."
    message =  {
            'contentType': 'PlainText',
            'content': text
        }
    fulfillment_state = "Fulfilled"    
    return close(intent_request, session_attributes, fulfillment_state, message)
```

---

## 💡 Flow with Screenshots

### Step 1: Define Intents
<img width="2505" height="868" alt="image" src="https://github.com/user-attachments/assets/0516e06b-a22d-4b47-9f86-6dc2f396e8c8" />


### Step 2: Lambda Integration
<img width="2542" height="1183" alt="lambda code" src="https://github.com/user-attachments/assets/cd7d593c-b37f-4f99-b21f-25b0abc441ef" />


### Step 3: Testing in Lex Console
<img width="545" height="810" alt="Screenshot 2025-10-16 162440" src="https://github.com/user-attachments/assets/8515f19d-91da-47cc-bf2f-6e073b6fac07" />
<img width="602" height="1034" alt="image" src="https://github.com/user-attachments/assets/3b8cbdfb-a0de-424f-80f9-3b9a96dedf69" />
<img width="720" height="1272" alt="image" src="https://github.com/user-attachments/assets/35060803-98f7-4bc7-bec8-3f816e9b0306" />



### Step 4: Monitoring with CloudWatch
<img width="1362" height="1145" alt="image" src="https://github.com/user-attachments/assets/fffea021-7026-48cf-bae2-afbda7174aa5" />


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
Data & AI Analyst | Snowflake Certified  

🔗 [LinkedIn](https://linkedin.com/in/vaishnavimule18) • [GitHub](https://github.com/vaishnavimule)
