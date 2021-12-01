[[Message Queue的特性]]
- 系統可用性降低
	- 因為變成Message Queue介接，所以如果Message Queue掛掉，其他跟它介接的系統通信也就掛掉了

- 系統複雜性提高
	- 引入MQ之後就要考慮以下幾點
		- 怎麼處理message丟失的問題
		- 怎麼保證message沒有被重複被consume
		- 怎麼保證訊息傳遞的順序

- 一致性
	- 如何保證發送message的系統A和Consum message的系統B，要馬都成功，要馬都失敗?