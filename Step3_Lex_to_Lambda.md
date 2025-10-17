# 💬 Step 3 – Connect Your Lex Chatbot to Lambda

## 🧩 Setting up your AWS Lambda function

<img width="1829" height="1062" alt="image" src="https://github.com/user-attachments/assets/be2e2bac-a4d4-4346-af70-37f82725ae8f" />

lambda_function.py (When someone asks about their account balance to your chatbot, Lex will ask your Lambda function to run this code, which will pick a random number to pretend it's the balance.

Lambda will pass this random number to Lex, who will then push the bank balance figure to the user through your chatbot.)

<img width="1027" height="1107" alt="image" src="https://github.com/user-attachments/assets/bb0252ec-72b4-4e28-9419-be094c775eb2" />

<img width="1543" height="757" alt="image" src="https://github.com/user-attachments/assets/08c75210-8e31-4a9d-9734-230b2eecf264" />

## 🧩 Connect AWS Lambda with Amazon Lex
Head back to your Amazon Lex console.
Select BankerBot.
On the left-hand menu, choose Aliases.

<img width="1108" height="781" alt="image" src="https://github.com/user-attachments/assets/5e9a9917-7054-49d8-a9a9-6515b3e7bfcf" />


## 🧩 Connect CheckBalance intent with your Lambda function

<img width="1093" height="436" alt="image" src="https://github.com/user-attachments/assets/9b5267de-7b24-4e6b-bf7f-1c198fd5214d" />


<img width="532" height="709" alt="image" src="https://github.com/user-attachments/assets/521e4226-213e-414a-9122-8ce33b21bb79" />

---
