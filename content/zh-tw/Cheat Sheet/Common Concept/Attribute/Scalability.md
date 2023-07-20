---
title: "伸縮性"
weight: 1
---

### 描述

由於系統使用量的多變化性，架構設計會考慮其各項需求伸縮的容易度。易於伸縮的系統可依照需求即時調整。在系統需求量高時，增加資源以快速消化需求。在系統需求量低時，減少資源以節約成本。在系統的各方面都需要考慮伸縮性，包含計算、檔案讀寫、資料庫讀寫、網路流量等。

### 常用作法

- 需求量規劃：按照目前使用量，預測未來增長、及特殊事件下的需求量，以決定系統伸縮設計方式
- 垂直伸縮：在單一伺服器上增加更多系統資源。伸縮速度較慢，伸縮彈性較小。
- 水平伸縮：伸縮至多台伺服器。伸縮速度較快，伸縮彈性大。
- 自動伸縮：動態偵測系統需求量，自動進行伸縮。