# 使用命令列介面(cmd)編譯程式
以下是C、C++、Java、Python的編譯方式

( 要記得先新增環境變數的PATH喔！ )

## C
+ `gcc 檔名.c`

+ `a.exe`

## C++
只有一個cpp檔的時候：

+ `g++ -o 檔名 檔名.cpp`

+ `./檔名`

有兩個或以上的cpp檔的時候：

+ `g++ -c -o 檔名1.o 檔名1.cpp`

+ `g++ -c -o 檔名2.o 檔名2.cpp`

+ `g++ -o 執行檔名稱 檔名1.o 檔名2.o`

+ `./執行檔名稱`

## Java
+ `javac 檔名.java`

+ `java 檔名`

## Python
+ `activate base`

+ `python 檔名.py`

# 補充
將c++的版本設為c++11：

+ `g++ -std=c++11`

可使編譯執行的指令不出現在介面上(加在最上面)

+ `@echo off`

可使程式不會一次執行完，必須按任意鍵才能繼續

+ `pause`

可自己建立一個執行檔(.bat)：
+ 將指令直接打進bat檔裡面

+ 點開bat檔就可以直接執行
