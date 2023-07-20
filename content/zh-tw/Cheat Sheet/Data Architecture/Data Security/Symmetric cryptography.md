---
title: "對稱加密"
weight: 1
---

### **描述**

對稱加密是一種加密技術，使用同一把金鑰對資料進行加密和解密。

### **使用情境**

- 對稱加密適用於需要提供高效的資料加密機制的場景，通常結合安全的金鑰傳遞機制以防止金鑰洩露。

### **優點**

- 加解密速度快，適合用於傳輸資料。

### **缺點**

- 由於加密和解密使用同一把金鑰，如果通過網路傳輸金鑰，會存在安全性問題。
- 可以使用金鑰交換技術安全地生成共享金鑰，例如：
    1. 使用RSA加密金鑰傳輸。
    2. 使用Diffie-Hellman演算法生成相互通訊的金鑰。

### **案例**

- DES (Data Encryption Standard) ：(過時) 由於DES算法已可被暴力破解，現已不推薦使用。
- AES (Advanced Encryption Standard)