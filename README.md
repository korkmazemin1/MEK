# MEK
this area is repository that ı try something about programming.



#include <stdio.h>
#include <conio.h>
#include <stdlib.h>
#include <time.h>

int a,b,c,sayi,t;

int toplama(){
	
	printf("toplamak istediginiz sayilari giriniz:");
	scanf("%d",&a);
	scanf("%d",&b);
	c=a+b;
	printf("verdiginiz saylarin toplami=%d",c);

    
}


int cikarma(){
	printf("cikarmak istediginiz sayilari giriniz:\n");
	scanf("%d",&a);
	scanf("%d",&b);
	c=a-b;
	printf("verdiginiz sayilarin cikarimi=%d\n",c);

    
}
int carpma(){
	printf("carpmak istediginiz sayilari giriniz:\n");
	scanf("%d",&a);
	scanf("%d",&b);
	c=a*b;
	printf("verdiginiz sayilarin carpimi=%d\n",c);

   
}
int bolme(){
	printf("bolmek istediginiz sayilari giriniz:\n");
	scanf("%d",&a);
	scanf("%d",&b);
	c=a/b;
	printf("verdiginiz sayilarin bolumu=%d\n",c);

    
}





int hesap(){
	int a,b,c;
	printf("yapmak istediginiz islemi seçiniz:\n1.TOPLAMA\n2.CIKARMA\n3.CARPMA\n4.BOLME\n");
	scanf("%d",&a);
	 
	 switch (a){
	     
	 case 1 :
	 	 toplama();
	 	break;
	 case 2 :
	 	cikarma();
	 	break;
	 case 3 :
	 	carpma();
	 	break;
	 case 4 :	
	bolme(); 
	    break;
	default:
		printf("lutfen verilen seceneklerden birini seciniz\n" );
		 break;
}
}

int sayitahmin(){
	int n;
	
	printf("lutfen [0-100] aralıgında bir sayı giriniz\n");
	srand(time(0));
	sayi = rand() % 101 ;
	for(t=0;t<100;t++){
			scanf("%d",&a);
	if(a==sayi){
		 printf("tebrikler nokta atışı");
		 break;
	}
	else if  (a<=sayi){
		printf("azıcık yukarı çık aslan");
	} 
	else if  (a>=sayi) printf("azıcık aşağı in aslan");
	else printf ("aralık içinde bir değer gir kör müsün canım");

	}
}


int main(){
	
	
	
	
	

	
	hesap();
	
	sayitahmin();
	
	
	
	
	return 0;
	
	
}
	
	
	






