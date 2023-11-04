#include <stdio.h>
int main (void)
{	int i=0, s1=0, s2=0, s3=0, s4=0, s5=0;
	unsigned int kisi,yas;
	double tl1,tl2,tl3,tl4,tl5,tutar;
	
	printf("Ailedeki birey sayisi kac?\n");
	scanf("%d",&kisi);
	printf("%d kisinin yaslarini giriniz:\n",kisi);
	
	while(i<kisi)
	{	scanf("%d",&yas);
		i++;
		if((yas<=10) && (yas>=1))
		{	s1++;
			tl1=s1*1;
		}
	    if((yas<=17) && (yas>=11))
		{	s2++;
			tl2=s2*1.5;
		}
		if((yas<=26) && (yas>=18))
		{	s3++;
			tl3=s3*4.75;
		}
		if((yas<=50) && (yas>=27))
		{	s4++,
			tl4=s4*7;
		}
		if(yas>=51) 
		{	s5++;
			tl5=s5*5.25;
		}		
	}
	tutar=tl1+tl2+tl3+tl4+tl5;
	printf("Odenecek toplam ucret %.2lf",tutar);
	
	return 0;
			
}
