# Phoenix - Secure E-Commerce Payment System
## Description:
Phoenix is a secure e-commerce application system involving Merchant and Payment Gateway servers (Java), and mobile client (Android).
The system is based on Secure Electronic Transaction (SET) which uses the concept of dual signature. The user registers and logs in using the Android application. After logging in, he selects the product he wants to buy and gets directed to the payment page. He then sends his card information to the merhchant server. The merchant server verifies the order and forwards the card details to the payment gateway. The gateway processes the card information and sends a one-time password as a SMS to the user. The user enters the password in the application and sends it back. The gateway verifies it and notifies the merchant which then sends a confirmation mail and message to the user.
## Key Components:
1. RSA encyption with 512 bit keys.
2. MD-5 hashing.
3. X.509v1 certificates.
4. Dual signatures
5. Use of salt and HMAC SHA-1 for storing passwords.
6. Use of timestamps and session keys.
## Libraries used:
1. Certificates - Bouncy Castle
2. Database - SQLite JDBC
3. SMS - Twilio
4. Email - Javamail
5. Cryptography - Java Cryptography Architecture
## Implementation:
### 1. Registration of new user:
![Registration_1](/Images/Registration_bd.PNG?raw=true)
![Registration_2](/Images/Registration_mobile.PNG?raw=true)
### 2. User login:
![Login_1](/Images/Login_bd.PNG?raw=true)
![Login_2](/Images/Login_mobile.PNG?raw=true)
### 3. Product Selection:
![Product_1](/Images/Product_bd.PNG?raw=true)
![Product_2](/Images/Product_mobile.PNG?raw=true)
### 4. Client-Merchant exchange:
![CM_1](/Images/Client_Merchant_bd.PNG?raw=true)
![CM_2](/Images/Payment_mobile.PNG?raw=true)
### 5. Client-Payment Gateway exchange:
![CP_1](/Images/Client_PG_bd.PNG?raw=true)
![CP_2](/Images/OTP_mobile.PNG?raw=true)
### 6. Payment Gateway-Merchant exchange:
![PM_1](/Images/PG_merchant_bd.PNG?raw=true)
### 7. Mechant-Client exchange:
![MC_1](/Images/email_mobile.PNG?raw=true)
