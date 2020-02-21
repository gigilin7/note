<font color="red">從輸出結果的 **注意** 中可看出不同</font>

# call by value
```c++
void add(int n)	
{
	cout<<"加1前："<<n<<endl;
	n=n+1;
	cout<<"加1後："<<n<<endl;
}
int main()
{
	int x=1;
	cout<<"原始："<<x<<endl;
	add(x); //x是一個新的記憶體空間 
	cout<<"現在："<<x<<endl;
	
} 
```
```
輸出結果：
原始：1
加1前：1
加1後：2
現在：1   <---注意
```
# call by reference(有兩種方式)
+ 第一種
```c++
void add(int *n)	
{
	cout<<"加1前："<<*n<<endl;
	*n=*n+1;
	cout<<"加1後："<<*n<<endl;
}
int main()
{
	int x=1;
	cout<<"原始："<<x<<endl;
	add(&x); //傳入x的位址 
	cout<<"現在："<<x<<endl;
	
}
```
```
輸出結果：
原始：1
加1前：1
加1後：2
現在：2   <---注意
```
+ 第二種
```c++
void add(int &n)	
{
	cout<<"加1前："<<n<<endl;
	n=n+1;
	cout<<"加1後："<<n<<endl;
}
int main()
{
	int x=1;
	cout<<"原始："<<x<<endl;
	add(x); //傳入x的位址 
	cout<<"現在："<<x<<endl;
	
} 
```
```
輸出結果：
原始：1
加1前：1
加1後：2
現在：2   <---注意
```
