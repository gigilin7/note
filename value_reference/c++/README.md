#include <iostream>
using namespace std;
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