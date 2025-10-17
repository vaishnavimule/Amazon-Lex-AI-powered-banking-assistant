# 📊 Step 4 –  Save User Info with Your Lex Chatbot


---

## 🧩 Remember information stored in CheckBalance
In your CheckBalance intent page, scroll down to the Contexts panel.
Under the Output contexts drop-down, choose New context tag.

<img width="1041" height="585" alt="image" src="https://github.com/user-attachments/assets/25d14610-5f50-4b8a-b406-7b2d4b105113" />

Name your new context contextCheckBalance

<img width="828" height="447" alt="image" src="https://github.com/user-attachments/assets/d5a2dbf0-5c66-4287-b7a6-c29cbcc4b858" />

Choose Add.

Choose Save intent.

Choose Build


### 🖼️ Create the FollowupCheckBalance intent


Name: FollowupCheckBalance

Description: Intent to allow a follow-up balance check request without authentication.


<img width="516" height="158" alt="image" src="https://github.com/user-attachments/assets/4ffa237f-96e6-4f7a-9cf2-efb667b8654e" />

1) Add a new slot:

Name: accountType

Prompt: For which account would you like your balance?

Slot type: accountType

2) Add another new slot:

Name: dateOfBirth

Prompt: For verification purposes, what is your date of birth?

Slot type: AMAZON.Date

Choose Save intent.
---

## 🔍 

<img width="1181" height="1048" alt="image" src="https://github.com/user-attachments/assets/eda0dccf-0571-4d07-921e-2d6f5776354d" />

<img width="602" height="1034" alt="image" src="https://github.com/user-attachments/assets/26f0368b-58ec-4de0-941d-bca8b80092fe" />

---

