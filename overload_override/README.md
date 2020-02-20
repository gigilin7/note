Overload多載
用相同的function名稱，但會根據你傳入參數的型別或數量不同，而呼叫相對應的function，舉例，當我呼叫A(1)，會印出字串"a1"，而當我呼叫A(1,100)，會印出字串"a2"

public void A(int i) { Systm.out.println("a1"); } 
public void A(int i,int j) { Systm.out.println("a2"); } 




Override覆載
實踐多形(polymorphism)的概念，在繼承中讓子類別"重新定義"父類別的方法

public class main
{
	public static void main(String[] args)
	{
		new Triangle().call();
	}
}
class Father
{  
    public void call()  
    {  
        Systm.out.println("I'm a father");
    }  
}  
  
class Child extends Father
{  
    public void call()  
    {  
        Systm.out.println("I'm a child");  
    }  
}  

在子類別可用super呼叫父類別的方法
public class main
{
	public static void main(String[] args)
	{
		new Triangle().call();
	}
}
class Father
{  
    public void call()  
    {  
        Systm.out.println("I'm a father");
    }  
}  
  
class Child extends Father
{  
    public void call()  
    {  
	super.call();
        Systm.out.println("I'm a child");  
    }  
}  