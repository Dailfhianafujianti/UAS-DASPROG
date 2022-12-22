# Ujian Akhir Semester 
Mata Kuliah 	:Dasar Pemograman
Nama	      	:Dailfhiana Fujianti
NIM	        	:	1227050032
Jurusan	    	:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Matriks merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). perkalian matriks memiliki syarat yaitu jumlah kolom matriks pertama sama dengan jumlah baris matriks kedua
Array merupakan tipe data terstruktur yang berguna untuk menyimpan sejumlah data yang bertipe sama. Bagian yang menyusun array disebut elemen array(isi), yang masing-masing elemen dapat diakses tersendiri melalui indeks array.
Tujuan utama dari source code kali ini yaitu menginputkan nilai dan mengubah suatu baris menjadi kolom dalam array 2 dimensi.
Bentuk dari array 2 dimensi adalah kita membuat 2 tanda [](bracket) tersebut.
Adapun logaritma dari source code ke 1 yaitu :
1.User menginputkan banyak baris yang diinginkan pada array
2.User menginputkan banyak kolom yang diinginkan pada array
3.User menginputkan satu persatu nilai array, dimulai dari baris ke 1 dan kolom ke 1
4.Nilai array akan ditampilkan sesuai aturan matriks
5.Lalu setelah itu ditamoilkan nilai dalam array yang sudah dibalik, dari baris menjadi kolom.
Dan logaritma dari source code ke 2 yaitu :
1.User menginputkan banyak  baris pada array mulai dari range 0-20
2.User menginputkan banyak kolom pada array mulai dari range 0-20
3.User mengimputkan satu persatu nilai array dimulai dari baris1 dan kolom1
4.Nilai array akan ditampilkan sesuai aturan matriks 
5.Nilai diavalidasi kembali apakah nilai tersebut habis dibagi 3,5,7
6.Apabila nilai tadi habis dibagi 3,5,7,maka nilai tidak akan ditampilkan.
  Apabila tidak habis, tampilkan kembali kepada user.


## Source Code
Source Code 1

      #include <iostream>
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


      cout << "====Array yang sebelum ditukar barisnya==== " << endl;

      for (i = 0; i < baris; i++){
      for (j = 0; j < kolom; j++){
      cout << " " << input [i][j];
      }
      cout << endl;
      }


      cout << "\n====Array yang sudah ditukar barisnya====" << endl;

      for (i = 0; i < kolom; i++){
      for (j = 0; j < baris; j++){
      cout << " " << input[j][i];
      }
      cout << endl;
      }

      }

      Source Code 2
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
  ![Screenshot (22)](https://user-images.githubusercontent.com/121110186/209096589-8efc9fa3-8b1d-49b4-b71a-2cd16c32801f.png)
![Screenshot (23)](https://user-images.githubusercontent.com/121110186/209096623-28caade2-2a8a-4b10-b582-e67711ad78f7.png)

               
