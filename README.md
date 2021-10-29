#include<stdio.h>
#include "luas.h"

int main(){
	//data
	float s,r,t,p,l;
	float Lkubus,Vkubus;
	float Vtabung,Ltabung;
	float Vbalok,Lbalok;
	
	printf("\t\t\t\t\t:::::::::::::TUGAS MODUL 2::::::::::::::\n");
	//masukaan data
	//kubus
	printf("KUBUS\n\n");
	printf ("masukkan nilai sisi       :   \t");
	scanf ("%f",&s);

	Lkubus =luas_kubus(s);
	printf("luas kubus = %.2f\n",Lkubus);
	
	Vkubus =volume_kubus(s);
	printf("volume kubus = %.2f\n",Vkubus);
	
	printf("==============================================\n");
	
	//tabung
	printf("TABUNG\n\n");
	printf ("masukkan nilai jari jari  :  \t");
	scanf("%f",&r);
	
	printf ("masukan nilai tinggi      :  \t");
	scanf("%f",&t);

	
	Vtabung = volume_tabung(r,t);
	printf("volume tabung = %.2f\n",Vtabung);
	
	Ltabung =luas_tabung(r);
	printf("luas tabung = %.2f\n",Ltabung);
	
	printf("==============================================\n");
	
	//balok
	printf("BALOK\n\n");
	printf ("masukan nilai tinggi      :  \t");
	scanf("%f",&t);
	
	printf ("masukkan nilai panjang    :  \t");
	scanf("%f",&p);
	
	printf("masukkan nilai lebar      :  \t");
	scanf("%f",&l);
	
	Vbalok = volume_balok(p,l,t);
	printf("volume balok = %.2f\n",Vbalok);
	
	Lbalok =luas_balok(p,l,t);
	printf ("luas balok = %.2f\n",Lbalok);
	
	//biodata
	printf("=================================\n");
	printf("Nama : YUSRIL IHZA SAPUTRA\n");
	printf("NIM  : 202110370311143");
	
	return 0;
}
