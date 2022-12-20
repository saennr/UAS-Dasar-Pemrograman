# Ujian Akhir Semester 
Mata Kuliah 	: Dasar Pemrograman
Nama	      	: Siti Aenurohmah
NIM		        :	1227050127
Jurusan	    	:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Definisi Matriks, Matriks merupakan suatu susunan bilangan real atau bilangan kompleks (atau elemen-elemen) yang disusun dalam baris dan kolom sehingga membentuk jajaran persegi panjang. Suatu matriks dinotasikan dengan huruf kapital seperti A,B,C dan seterusnya, sedangkan anggotanya dengan huruf kecil. Baris itu susunannya horizontal atau ke samping, sedangkan kolom susunannya vertikal atau dari atas ke bawah.

## Source Code
#include <iostream>
using namespace std;

int main() {
	
	cout<<"====================================="<<endl;
	cout<<"        PROGRAM ARRAY 2 DIMENSI      "<<endl;
	cout<<"====================================="<<endl;
	cout<<" Nama  : Siti Aenurohmah "<<endl;
	cout<<" NIM   : 1227050127 "<<endl;
	cout<<" Kelas : IF-C "<<endl;
	cout<<"~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"<<endl<<endl;
	
	cout<<"-------------------------------------------------------------------------------------"<<endl;
	cout<<" 1. BARIS DAN KOLOM, NILAI DIINPUTKAN DAN DIBALIK KOLOM JADI BARIS, BARIS JADI KOLOM "<<endl;
	cout<<"-------------------------------------------------------------------------------------"<<endl;
	
	int A[100][100];
	int baris, kolom, b, k;
	
	cout<<"Masukan jumlah baris : ";
	cin>>baris;
	cout<<"Masukan jumlah kolom : ";
	cin>>kolom;
	cout<<endl;
	
	for (b=1;b<=baris;b++){
		for (k=1;k<=kolom;k++){
			  cout<<"Baris["<<b<<"]Kolom["<<k<<"] = ";
			  cin>>A[b][k];
		}
		cout<<endl;
	}
	cout<<"Matriks A "<<endl;
	for (b=1;b<=baris;b++){
		for (k=1;k<=kolom;k++){
			 cout<<A[b][k]<<" ";
		}
		cout<<endl;
	}
	cout<<endl<<"Matriks dibalik kolom jadi baris, baris jadi kolom "<<endl;
	for (b=1;b<=kolom;b++){
		for (k=1;k<=baris;k++){
			 cout<<A[k][b]<<" ";
		}
		cout<<endl;
	}
	
	cout<<"----------------------------------------------------------------------------"<<endl;
	cout<<"            2. MENAMPILKAN BILANGAN YANG HABIS DIBAGI 3,5,7 "<<endl;
	cout<<"----------------------------------------------------------------------------"<<endl;	
	
	cout<<"Masukan jumlah baris : ";
	cin>>baris;
	cout<<"Masukan jumlah kolom : ";
	cin>>kolom;
	cout<<endl;
	
	for (b=1;b<=baris;b++){
		for (k=1;k<=kolom;k++){
			  cout<<"Baris["<<b<<"]Kolom["<<k<<"] = ";
			  cin>>A[b][k];
		}
		cout<<endl;
	}
	cout<<"Matriks A "<<endl;
	for (b=1;b<=baris;b++){
		for (k=1;k<=kolom;k++){
			 cout<<A[b][k]<<" ";
		}
		cout<<endl;
	}
	cout<<endl<<"Nilai Matriks A yang habis dibagi 3,5,7 "<<endl;
	for (b=1;b<=baris;b++){
		for (k=1;k<=kolom;k++){
			if(A[b][k]%3==0){
				cout<<"\t"<<A[b][k];
			}
			else if(A[b][k]%5==0){
				cout<<"\t"<<A[b][k];
			}
			else if(A[b][k]%7==0){
				cout<<"\t"<<A[b][k];
			}
			else {
			}
		}
		cout<<endl;
	}
	return 0;
}

## Output
=====================================
        PROGRAM ARRAY 2 DIMENSI
=====================================
 Nama  : Siti Aenurohmah
 NIM   : 1227050127
 Kelas : IF-C
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-------------------------------------------------------------------------------------
 1. BARIS DAN KOLOM, NILAI DIINPUTKAN DAN DIBALIK KOLOM JADI BARIS, BARIS JADI KOLOM
-------------------------------------------------------------------------------------
Masukan jumlah baris : 2
Masukan jumlah kolom : 3

Baris[1]Kolom[1] = 2
Baris[1]Kolom[2] = 3
Baris[1]Kolom[3] = 4

Baris[2]Kolom[1] = 5
Baris[2]Kolom[2] = 8
Baris[2]Kolom[3] = 9

Matriks A
2 3 4
5 8 9

Matriks dibalik kolom jadi baris, baris jadi kolom
2 5
3 8
4 9
----------------------------------------------------------------------------
            2. MENAMPILKAN BILANGAN YANG HABIS DIBAGI 3,5,7
----------------------------------------------------------------------------
Masukan jumlah baris : 2
Masukan jumlah kolom : 3

Baris[1]Kolom[1] = 1
Baris[1]Kolom[2] = 3
Baris[1]Kolom[3] = 2

Baris[2]Kolom[1] = 5
Baris[2]Kolom[2] = 9
Baris[2]Kolom[3] = 4

Matriks A
1 3 2
5 9 4

Nilai Matriks A yang habis dibagi 3,5,7
        3
        5       9
  
