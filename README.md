# 3.-odev

//girilen say�daki s�radaki fibonacci say�s�

#include<stdio.h>
int fib(int);
int main(void)
{
	int x;
	printf("bir sayi giriniz: ");
	scanf("%d" , &x);
	
	printf("sayiniz %d" , fib(x));
	
	return 0;
}

int fib(int x)
{
	int a=1 , b=1;
	int c;
	
	for(int i=3; i<=x; i++)
	{
		c=a+b;
		a=b;
		b=c;
	}
	return c;
}
