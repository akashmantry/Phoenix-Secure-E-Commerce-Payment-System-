# Phoenix-Secure-E-Commerce-Payment-System-
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
### 2. User login:
### 3. Product Selection:
### 4. Client-Merchant exchange:
### 5. Merchnat-Payment Gateway exchange:
### 6. Payment Gateway-Client exchange:
### 7. Payment Gateway-Merchant exchange:
### 8. Mechant-Client exchange:
