# ⚙️ Step 5 –  Build Complex Conversations with Multiple Slots


---

## 🧩 Create the new TransferFunds intent

Create a new empty intent with the following properties:

Name: TransferFunds

Description: Help user transfer funds between bank accounts

![1760730040198](image/Step2_Lambda_Function_Integration/1760730040198.png)

![1760730070135](image/Step2_Lambda_Function_Integration/1760730070135.png)

![1760730077607](image/Step2_Lambda_Function_Integration/1760730077607.png)


In the Confirmation prompt panel, enter the following:

Got it. So we are transferring {transferAmount} from {sourceAccountType} to {targetAccountType}. Can I go ahead with the transfer?

In Decline response, enter:


The transfer has been cancelled.

![1760730087376](image/Step2_Lambda_Function_Integration/1760730087376.png)

![1760730123782](image/Step2_Lambda_Function_Integration/1760730123782.png)

![1760730133071](image/Step2_Lambda_Function_Integration/1760730133071.png)
