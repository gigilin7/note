# pointer(指標)
**pointer指的就是記憶體的地址**

## 舉例：

把`記憶體`比喻成`一整條街的房子`

`每棟房子`都有自己的`門牌號碼(位址)`

而`指標變數`就是儲存`門牌號碼xxx的房子裡的東西`


## 用法：

`*`：指標變數的`內容` (記憶體的內容)

`&`：變數的`位址` (記憶體的位址)


## 實作：

```C
int a=1, b=2;

int *p;   //p是指向int的指標

p = &a;  // &a是取a的地址(也就是說，p現在跟a是指在同一個記憶體，所以內容也相同)

cout<<"a原始的值："<<a<<endl;
cout<<"b原始的值："<<b<<endl;

b = *p;  //b的值變成p所指到的記憶體的內容

*p = 0;  //將p指到的記憶體內容變為0(因為a跟p共用同一個記憶體，所以a的值也會跟著改變成0)

cout<<"a目前的值："<<a<<endl;
cout<<"b目前的值："<<b<<endl;

```
```
輸出結果：
a原始的值：1
b原始的值：2
a目前的值：0
b目前的值：1

```
