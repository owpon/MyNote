- Better performance
	- 非同步溝通
	- consumer 有空時才會處理Message


- Decouple
	- 訊息的發送方和接受方都不需要知道彼此，consumer和produce可以隨便你用不同語言實作，只要message的格式事先有溝通好，知道就好。
	-   publisher 與 consumer 不需要知道雙方的實際的位置(例如：IP address)，只要將資料往 message queue 送就好


-   Reliability
	-   因為資料是送到queue裡面，所以data不易丟失
	-   一但訊息被成功送進queue裡，在他被成功消耗掉之前，都會保存著，有時可能因為莫名原因，consumer都掛了，在consumer恢復之前，需要做的任務還留著，能夠等到恢復之後再繼續處理。


-   Flexiability of scaling
	- producer, queue, consumer 可以依照需求擴張或縮減


參考資料:
[讓任務排隊吧](https://medium.com/starbugs/%E8%AE%93%E4%BB%BB%E5%8B%99%E6%8E%92%E9%9A%8A%E5%90%A7-message-queue-1-de949e274c43)
[什麼是message queue](https://homuchen.medium.com/%E4%BB%80%E9%BA%BC%E6%98%AFmessage-queue-%E5%84%AA%E9%BB%9E%E5%8F%8A%E4%BD%BF%E7%94%A8%E5%A0%B4%E6%99%AF-23d6a39cc4f2)