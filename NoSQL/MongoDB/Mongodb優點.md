因為是NoSQL的DB，所以NoSQL的優點他都有

* Schema-less: Mongodb擁有很彈性的`schema`
* 易於擴展:因為本身是`document`的數據模型，所以能夠很容易在多台伺服器之間進行數據分割。
* 優秀的性能: MongoDB能預分配，以利用額外的空間換取穩定，同時盡可能把多的內存用作cache，試圖為每次查詢自動選擇正確的索引。