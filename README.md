# 🚀 zkLogin Demo on Sui Blockchain

A demonstration of **Zero-Knowledge Login (zkLogin)** implementation on the **Sui Blockchain**, enabling secure, privacy-preserving authentication via **Google**, **Twitch**, and **Facebook**. This project leverages **Zero-Knowledge Proofs (zk-SNARKs)** to protect user data while allowing seamless interaction with the Sui network.

---

## 📌 **Table of Contents**

- [🔑 Features](#-features)  
- [⚡ Tech Stack](#-tech-stack)  
- [⚙️ Setup Instructions](#-setup-instructions)  
- [🔐 Authentication Flow](#-authentication-flow)  
- [📝 License](#-license)  

---

## 🔑 **Features**

- **Secure Authentication** with Google, Twitch, and Facebook using **OpenID Connect (OIDC)**  
- **Real-Time SUI Balance Tracking** for authenticated accounts  
- **Transaction Execution** on the Sui network using **zkLogin signatures**  
- **Faucet Integration** to request SUI tokens on the Sui **Devnet**  
- **Session Management** with easy state clearing for better security  

---

## ⚡ **Tech Stack**

- **Frontend:** React, TypeScript  
- **Blockchain:** Sui Devnet, zkLogin Protocol  
- **Authentication:** OpenID Connect (OIDC)  
- **Cryptography:** Zero-Knowledge Proofs (zk-SNARKs)  

---

## ⚙️ **Setup Instructions**

### 1️⃣ **Clone the Repository**

```bash
git clone https://github.com/GillHapp/my-zklogin-project
cd my-zklogin-project
```

### 2️⃣ **Install Dependencies**

```bash
npm install
```

### 3️⃣ **Configure OpenID Credentials**

- Create a `config.json` file based on the provided `config.example.json`.  
- Add your **Google**, **Twitch**, and **Facebook Client IDs** along with **Sui network endpoints**.

### 4️⃣ **Run the Project**

```bash
npm start
```

- The app will be accessible at: [http://localhost:3000](http://localhost:3000)  

---

## 🔐 **Authentication Flow**

1. **User Authentication:**  
   The user selects an OpenID provider (Google/Twitch/Facebook) for login.  
   
2. **JWT Generation:**  
   After successful authentication, a **JWT (JSON Web Token)** is generated.  
   
3. **Zero-Knowledge Proof Request:**  
   The JWT is sent to the **prover service**, which returns a **Zero-Knowledge Proof**.  
   
4. **Secure Address Derivation:**  
   The user's **Sui address** is derived securely, ensuring no personal data is exposed.  
   
5. **Transaction Signing:**  
   Transactions are signed using **zkLogin credentials** and submitted to the Sui network.  

---

## 📜 **License**

This project is licensed under the [MIT License](LICENSE).

---
