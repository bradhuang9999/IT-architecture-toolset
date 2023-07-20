---
title: "非對稱性加密"
weight: 2
---

### **描述**

非對稱性加密是一種加密技術，與對稱性加密不同，它使用一對金鑰，包括公鑰和私鑰，來進行加密和解密操作。

運作方式如下：先產生一組公私鑰對。公鑰可以在網路上傳輸給其他人，但私鑰必須保密，不會在網際網路上傳輸。在加密過程中，傳送者使用私鑰對資料進行加密或數位簽名。接收者收到加密後的資料後，使用公鑰鑰對其進行解密或驗證簽名。如果解密或驗證成功，那麼可以確認該資料確實來自公鑰對應的私鑰，且在傳輸過程中沒有被篡改。

### **使用情境**

- **數位簽章：** 用於驗證檔案或資料的真實性和完整性，防止偽造或篡改。
- **訊息加密：** 用於保護敏感資訊在網路傳輸過程中的安全性，只有私鑰擁有者能夠解密讀取內容。
- **HTTPS訊息傳輸：** 用於對網站的傳輸資料進行加密，確保通訊過程中的隱私和安全。
- **安全傳輸對稱性加密金鑰：** 在對稱性加密中，用非對稱性加密演算法傳輸對稱加密的金鑰，確保金鑰在傳輸過程中不被洩露。

### **優點**

- **安全性較高：** 私鑰不會在網路上傳輸，只有私鑰持有者能夠解密或簽署資料，因此提供較高的安全性。
- **安全金鑰交換：** 可以用於安全地交換對稱加密演算法的金鑰，增加了整個系統的安全性。

### **缺點**

- **加解密速度較慢：** 與對稱性加密相比，非對稱性加密的演算法複雜性較高，因此需要更長的時間來完成加解密操作。

### **案例**

- **RSA（Rivest-Shamir-Adleman）**
- **DSA（Digital Signature Algorithm）**
- **ECC（Elliptic Curve Cryptography）**