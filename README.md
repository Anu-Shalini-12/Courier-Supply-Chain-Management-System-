# 🚚 Courier Supply Chain Management System using Hyperledger Fabric

## 📘 Project Overview

A blockchain-based system built using **Hyperledger Fabric** to revolutionize parcel tracking and courier supply chain operations. The system enhances **transparency**, **automation**, and **data integrity**, resolving the issues faced by traditional courier logistics.

---

## ❗ Problem Statement

Courier supply chains often suffer from:

- ❌ Lack of transparency and visibility  
- 📄 Manual, paper-based tracking  
- ⚠️ Error-prone processes  
- 🕵️‍♀️ Poor auditability and data security  

These challenges cause delivery delays, data mismatches, and loss of customer trust.

---

## 🎯 Project Objective

To develop a decentralized **Courier Supply Chain Management System** that:

✅ Enables real-time tracking of parcels  
✅ Automates and digitizes parcel management  
✅ Maintains a tamper-proof audit trail  
✅ Enhances operational efficiency and trust

---

## 🧰 Technologies Used

| Technology           | Purpose                                       |
|----------------------|-----------------------------------------------|
| **Hyperledger Fabric** | Blockchain framework for enterprise-grade networks |
| **Chaincode (Java)**   | Smart contract logic for parcel operations   |
| **Fabric CA**         | Identity and certificate management           |
| **CouchDB**           | State database for real-time ledger queries   |
| **Java SDK**          | Backend interaction with the blockchain       |
| **Practical Lab**     | Testing and simulation environment            |

---

## 🧠 Chaincode Functionalities

The core logic is implemented as **chaincode in Java** and deployed to the Fabric network:

| Function             | Description |
|----------------------|-------------|
| `InitLedger()`       | Initializes the ledger with demo parcel data |
| `AddParcel(id, sender, receiver, status)` | Adds a new parcel to the ledger |
| `QueryParcelById(id)` | Fetches parcel details by ID |
| `UpdateParcelStatus(id, newStatus)` | Updates the current status/location of a parcel |

---

## 🔁 Workflow Summary

1. 🛠️ **Admin initializes** the ledger using `InitLedger()`.
2. 📦 **New parcels** are added via `AddParcel(...)`.
3. 🔄 **Status updates** occur at each delivery milestone via `UpdateParcelStatus(...)`.
4. 🔍 **Users query** parcels at any time using `QueryParcelById(...)`.

All actions are **recorded immutably** on the ledger and reflected in **CouchDB** instantly.

---

## 🏗️ Hyperledger Fabric Architecture

| Component           | Role |
|---------------------|------|
| **Peers**           | Validate, endorse, and store transactions |
| **Orderer**         | Sequences transactions into blocks |
| **Certificate Authority (CA)** | Issues and verifies identities |
| **Chaincode**       | Contains the logic for parcel lifecycle |
| **Ledger**          | Stores immutable blockchain + current world state (CouchDB) |

---

## 💡 Features & Benefits

| Feature                   | Benefit                                        |
|---------------------------|------------------------------------------------|
| **Immutable Ledger**      | Prevents tampering and ensures auditability    |
| **Real-Time Status Updates** | Enhances trust and tracking visibility     |
| **Paperless Automation**  | Reduces human errors and manual work          |
| **Role-Based Access Control** | Secures access using digital identities  |
| **CouchDB Query Support** | Enables fast, key-based searches for parcels  |

---

## 🧪 Testing & Verification

All chaincode functions were thoroughly tested using:

- ✅ **CLI commands**  
- ✅ **Postman or Java SDK APIs**  
- ✅ **CouchDB** for real-time state verification  
- ✅ **Peer logs** for transaction confirmation  

📸 **Screenshots Proof** (as described in project):

| Operation        | Validation Method               |
|------------------|----------------------------------|
| `InitLedger()`    | Ledger pre-loaded with demo data |
| `AddParcel(...)`  | Successfully added new parcel    |
| `QueryParcelById()` | Retrieved correct parcel data  |
| `UpdateParcelStatus()` | Status reflected accurately |

---

## ✅ Conclusion

The **Courier SCM system using Hyperledger Fabric**:

- 📦 Automates and secures parcel lifecycle management  
- 🔗 Offers full **data transparency and traceability**  
- 🧾 Provides a **tamper-proof audit trail**  
- 🚀 Demonstrates scalable potential for enterprise-grade courier logistics  

---


