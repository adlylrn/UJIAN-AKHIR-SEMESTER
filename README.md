# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Adly Juliarta Lerian
<br>NIM		:	1227050007
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Topik utama dari kode sumber ini adalah membuat array dua dimensi menggunakan C++.
Tujuan utama dari source code ini adalah untuk mengubah posisi suatu nilai dari baris ke kolom dan sebaliknya.
<br> 1.Pengguna memasukkan berapa banyak baris yang berisi tabel.
<br> 2.Pengguna memasukkan berapa banyak baris dan kolom yang terdapat dalam tabel. 
<br> 3.Pengguna memasukkan nilai tabel secara berurutan dari baris 1 dan kolom 1.
<br> 4.Jika ya, nilai tabel ditampilkan sesuai dengan aturan matriks.
<br> 5.Kemudian nilai tabel yang dibalik ditampilkan, dari baris ke kolom dan sebaliknya.
## Source Code
codingan (1)
#include<iostream>
using namespace std;

int main()
{
	int input [100][100];
	int baris, kolom, i, j;
	
	cout << "Imput jumlah baris : ";
	cin >> baris;
	cout << "Input jumlah kolom : ";
	cin >> kolom;
	cout << endl;
	
	for (i = 0; i < baris; i++){
		for (j = 0; j < kolom; j++){
			cout << "baris" << i+1 << ",kolom" << j+1 << " = ";
			cin >> input[i][j];
		}
		cout << endl;
	}
	
	cout << "Hasil : "<<endl;
	
	for (i = 0; i < baris; i++){
		for (j = 0; j < kolom; j++){
			cout << " " << input [i][j];
		}
		cout << endl;
	}
	
	cout << "=======================" << endl;
	
	for (i = 0; i < kolom; i++){
		for (j = 0; j < baris; j++){
			cout << " " << input[j][i];
		}
		cout << endl;
	}
  
  codingan (2)
  #include <iostream>
using namespace std;

int main (){
	int A [20][20];
	int b, k, i, j;
	cout << "Masukkan jumlah baris : ";
	cin >> b;
	cout << "Masukkan jumlah kolom : ";
	cin >> k;
	
	for (i=0;i<=b-1;i++) {
		for(j=0;j<=k-1;j++) {
			cout << "Masukkan nilai (" << i << "." << j << ") : ";
			cin >> A [i][j];
		}
	}
	cout << "Nilai yang diinputkan : \n";
	for(int i = 0; i < b; i++){
		for(int j = 0; j < k; j++){
			cout<<A[i][j]<<"\t";
		}
		cout<<endl;
	}
	int angka[20];
	int index = 0;
	for(i=0;i<b;i++){
		for(j=0;j<k;j++) {
			if (A [i][j]%3 != 0 && A[i][j]%5 != 0 && A[i][j]%7 != 0){
				angka[index] = A[i][j];
				index++;
			}
		}
	}
	cout<<"Angka yang tidak bisa dibagi 3, 5, 7 adalah ";
	for(int i = 0; i < index; i++){
		cout<<angka[i]<<", ";

	}
}
## Output
screenshoot(1)
![Screenshot (23)](https://user-images.githubusercontent.com/121163818/209268835-30e59e61-3ac3-4bbf-ad3f-fcfc07b58d75.png)

screenshoot(2)
![Screenshot (24)](https://user-images.githubusercontent.com/121163818/209269471-e0ebe9b0-5fed-4473-b1f7-6790cde6a9bd.png)
