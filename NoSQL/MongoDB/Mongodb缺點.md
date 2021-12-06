因為NoSQL的特性，缺點也是很明顯
* 不支援事務(transaction)操作:所以不能用在需要操作錯誤就返回原樣的機制，因為不保證一致性
* 占用較多的空間:因為它會為了效能預先分配空間，而且為了有彈性給存入的`document`資料結構，會開出一塊空間給那些欄位。


參考來源:
[MongoDB基礎](https://ithelp.ithome.com.tw/articles/10184679)