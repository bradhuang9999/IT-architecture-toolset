---
title: "Partition"
weight: 5
---

### **描述**

Partition是將一個巨大的資料表根據時間、字母、數字或Hash值等方式設定分區鍵(Partition key)，並使用該分區鍵將資料表分割並存儲於同一伺服器上的多個不同硬碟或磁碟陣列中。

### **使用情境**

- 當單一資料表過大且存在明確可用的分區鍵時。
- 希望能夠在單一伺服器上分散單一資料表過大的負擔。

### **優點**

- 查詢效能優化：資料查詢可以分散在多個硬碟上，提升查詢效能。
- 架構簡單：無需使用複雜的分散式多伺服器資料庫管理架構。

### **缺點**

- 單點故障：當單一分區或伺服器發生故障時，該分區的資料將無法存取。
- 資料不均衡風險：若分區鍵設計不當，可能導致資料分佈不平衡，使部分硬碟處於閒置狀態。
- 管理複雜性：需要考慮跨分區查詢、資料一致性、備份、故障恢復等議題
