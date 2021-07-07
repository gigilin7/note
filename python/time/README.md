# 使用 time 得到系統當前時間
```xml
import time
while True:
    localtime = time.localtime()
    result = time.strftime("%Y-%m-%d %I:%M:%S %p", localtime)
    print(result)
    time.sleep(1)
```

## 輸出如下：
```
2021-07-07 11:24:13 AM
2021-07-07 11:24:14 AM
2021-07-07 11:24:15 AM
2021-07-07 11:24:16 AM
2021-07-07 11:24:17 AM
2021-07-07 11:24:18 AM
^C
```


# 使用 datetime 得到系統當前時間
```xml
from datetime import datetime
result = datetime.now().strftime("%Y-%m-%d %I:%M:%S %p")
print(result)
```

## 輸出如下：
```
2021-07-07 11:39:33 AM
```

# strftime 常用的格式化字串
```
格式化符號	說明
%Y	四位數的年份（000-9999）
%y	兩位數的年份（00-99）
%m	月（01-12）
%d	日（01-31）
%H	24 小時制的小時（00-23）
%I	12小時制的小時（01-12）
%M	分鐘（00-59）
%S	秒（00-59）
%p	AM或PM
```

