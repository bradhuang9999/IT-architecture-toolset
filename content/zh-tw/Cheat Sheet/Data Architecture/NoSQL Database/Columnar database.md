---
title: "列式資料庫"
weight: 2
---

### **描述**

列式資料庫(Columnar Database) 以Column為單位儲存資料，因此若目標是僅需要抓取少數欄位進行分析，可以快速取得所需欄位的數值。
例如，對於銷售資料中的許多明細欄位，其中有兩個欄位：商品編號和銷售金額。
這些欄位被分開儲存，因此若想要取得特定商品的銷售金額，只需要掃描商品清單的欄位，找到目標商品的對應行索引（row idx）。
然後使用該行索引篩選銷售金額欄位的對應數值資料，即可取得該商品的銷售金額。
由於資料存放時，未使用的欄位是分開存放的，所以資料讀取速度比基於行的傳統資料庫更快。

### **使用情境**

- 即時的大數據分析系統

### **優點**

- 彙總特定欄位速度快：由於各欄位分開存放，可以快速取出各欄位的彙總資料。
- 可快速寫入：相對於傳統OLAP資料庫，可以即時將資料存放於各個欄位，滿足即時大數據分析需求。
- 易於水平擴展：由於各欄位分開存放，可以將資料存放於其他伺服器上，提高可用性。

### **缺點**

- 在彙總較多欄位時，效率可能會比傳統基於行的資料庫差。

### 案例

- Apache Cassandra
- Amazon Redshift
- Google BigQuery
- Vertica
- Apache Parquet