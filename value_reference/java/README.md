# Call by value
```java
class Value
{
	public static void main ( String[] args ) 
	{
      		int x =1;
      		System.out.println ("原始："+x);
      		add(x);
      		System.out.println ("現在："+x);
	}

	public static void add(int n) 
	{
      		System.out.println ("加1前："+n);
      		n=n+1;
      		System.out.println ("加1後："+n);
	}
}
```
```
輸出結果：
原始：1
加1前：1
加1後：2
現在：1
```

# Call by reference
```java
class Number {
   int x;
}
class Reference {

   public static void main ( String[] args ) {
      Number num = new Number();
      num.x=1;
      System.out.println("原始："+num.x);
      add(num);
      System.out.println("現在："+num.x);
   }

   public static void add(Number n) {
      System.out.println("加1前："+n.x);
      n.x=n.x+1;
      System.out.println("加1後："+n.x);
   }
}
```
```
輸出結果：
原始：1
加1前：1
加1後：2
現在：2
```
