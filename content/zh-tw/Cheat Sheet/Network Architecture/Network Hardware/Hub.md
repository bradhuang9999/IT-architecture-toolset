---
title: "Hub"
weight: 1
---

### 描述

Hub讓區域網路中的多台設備可以互相溝通，其工作原理十分單純，只要收到任何一個封包都會廣播連接到同一Hub的其他電腦。但是由於一次只可以傳輸一個設備的封包，因此除非只有要連接少數設備，否則已經較少使用。

### 優點

- 價格低廉：由於工作原理單純，因此設備價格較低
- 設定單純：無須在Hub上進行任何設定，只要各台設備的IP沒有衝突即可互相溝通。

### 缺點

- 無法同時連接太多設備：由於其固定廣播特性，容易造成封包碰撞，同時只有辦法傳輸一個封包。
- 安全性較低：由於固定廣播封包，其他設備都會收到封包內容，因此未經授權者可用此方式監聽封包內容。