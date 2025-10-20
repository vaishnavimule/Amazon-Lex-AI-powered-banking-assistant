# ⚙️ Step 5 –  Build Complex Conversations with Multiple Slots


---

## 🧩 Create the new TransferFunds intent

Create a new empty intent with the following properties:

Name: TransferFunds

Description: Help user transfer funds between bank accounts

<img width="929" height="565" alt="image" src="https://github.com/user-attachments/assets/aaca980a-c5f3-4ef5-9183-c1dfc068cefe" />

<img width="1078" height="253" alt="image" src="https://github.com/user-attachments/assets/cb13338d-441c-4ddb-8334-83000bef3356" />

<img width="1170" height="595" alt="image" src="https://github.com/user-attachments/assets/a435cfea-ce2c-4d88-a523-26b046162c92" />

In the Confirmation prompt panel, enter the following:

Got it. So we are transferring {transferAmount} from {sourceAccountType} to {targetAccountType}. Can I go ahead with the transfer?

In Decline response, enter:


The transfer has been cancelled.

<img width="1193" height="715" alt="image" src="https://github.com/user-attachments/assets/5473ed2e-00a2-49f7-8576-fe01ca7d26f1" />

<img width="720" height="1272" alt="image" src="https://github.com/user-attachments/assets/60d8fdc3-9c3d-49d2-b58e-62b2e820712d" />

