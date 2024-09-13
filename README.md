# Dissertation 
**Privacy-Preserving Balancer for Payment Systems in the Trade Credit Market**
This project implements a secure system of balancing payments and sharing information among SMEs in the trade credit system using advanced cryptographic techniques. The project dives into different scenarios within the credit situations and optimizes them using privacy-preserving methods. It focuses on protecting the sensitive data of companies as well as making financial analyses on encrypted data using tools like federated learning, proactive secret sharing, and homomorphic encryption. 

# File Overview

**1. Symmetric_key.ipynb**
Implemented symmetric key encryption using the Fernet encryption method to protect the sensitive financial data of companies. A key-encryption key (KEK) has been generated to encrypt the symmetric key, to add an additional level of security.
We have extracted data from the financials of AALI and then converted them into a data frame for the experiment. 

**2. ProactiveSecretSharing.ipynb**
This file implements proactive secret sharing where financial data is divided into multiple shares and distributed among trusted parties. These shares are refreshed as well, ensuring no party can reconstruct the secret without enough valid shares. A (3,3) threshold has been used for the same. 

**3. Network_Visualizations.ipynb**
This file encrypts the business-to-business networks using the NetworkX library, using Python's Hashlib library. Besides this, proximity-based color gradients have also been applied to visualize how close the suppliers are to the companies taken into consideration.

**4. Homomorphic_Encryption.ipynb**
Here the code is based on the CKKS(Cheon-KIm-Kim-Song) scheme extracted from Python's TenSeal library for homomorphic encryption. This allows for computations on encrypted financial data without decrypting it. Example ratios included are Current Ratio, Debt-to-Equity, and Return on Assets.

**5. Federated_Learning.ipynb**
The code here mimics a Federated Learning setup where the financial data is distributed among SMEs, which are the local clients in the case. Each client trains their model locally on their data, and only the parameters are shared with the central server. In no part of the process, the raw data is transmitted, thus preserving the privacy of each SME.

