# Tugas2
Tugas2


### Penggunaan end


Di dalam sebuah fungsi "**print()**" bahasa python terdapat parameter "**end**". Parameter "**end**" adalah parameter yang digunakan untuk memasukan **string** atau 

**karakter** apapun untuk mengakhiri sebuah statement.  Secara default jika kita melakukan print dalam python, output akan dicetak dalam baris baru. Tapi jika kita 

memasukan fungsi "**end**" maka hasil output tidak akan langsung berada di garis baru.

Ini adalah Contoh kodenya :

### Penggunaan end
   
	print('A', end="")
   
	print('B', end="")
   
	print('C', end="")
	print()
   	
	print('X')
   
	print('Y')
   
	print('Z')

Gambar 1 :

![gambar1](https://user-images.githubusercontent.com/56499371/68083023-9a3f6800-fe56-11e9-804d-33efa71df45c.png)



### Penggunaan Separator

Separator "**sep**" dalam python digunakan sebagai pembatas antara output yang dihasilkan.


**Contoh Kode :**

    


	w, x, y, z = 10, 15, 20, 25
    
	print(w, x, y, z, sep=',')
    
	print(w, x, y, z, sep='')
    
	print(w, x, y, z, sep=':')
    
	print(w, x, y, z, sep='- - - - -')


**Output yang didapat :**

Gambar2 :

![Output_sep](https://user-images.githubusercontent.com/56499371/68083024-9c092b80-fe56-11e9-8397-5cbf6616137d.png)

Disini kita bisa mengisi **sep='isi_disini'** dengan string atau karakter apapun.



### Penggunaan string format


Didalam String format ini dapat digunakan ketika kita ingin mengatur dan memposiskan print output menjadi sedemikian rupa.


**Contoh kode :**


 # String yang belum di format
  
	print(0, 10 ** 0)
  
	print(1, 10 ** 1)
  
	print(2, 10 ** 2)
  
	print(3, 10 ** 3)
  
	print(4, 10 ** 4)
  
	print(5, 10 ** 5)
  
	print(6, 10 ** 6)
  
	print(7, 10 ** 7)
  
	print(8, 10 ** 8)
  
	print(9, 10 ** 9)
  
	print(10, 10 ** 10)



**Output :**

Gambar 3:

![Output_String](https://user-images.githubusercontent.com/56499371/68083025-9dd2ef00-fe56-11e9-8a1b-4ccea5d8cadc.png)

Disini saya akan membuat outputnya menjadi seperti berikut :

Gambar 4:


![Output_String2](https://user-images.githubusercontent.com/56499371/68083026-9f9cb280-fe56-11e9-945d-f75a280b9259.png)


**Dengan Kode :**

   

	print('{0:>3} {1:>16}'.format(0, 10 ** 0))
   
	print('{0:>3} {1:>16}'.format(1, 10 ** 1))
   
	print('{0:>3} {1:>16}'.format(2, 10 ** 2))
   
	print('{0:>3} {1:>16}'.format(3, 10 ** 3))
   
	print('{0:>3} {1:>16}'.format(4, 10 ** 4))
   
	print('{0:>3} {1:>16}'.format(5, 10 ** 5))
   
	print('{0:>3} {1:>16}'.format(6, 10 ** 6))
   
	print('{0:>3} {1:>16}'.format(7, 10 ** 7))
   
	print('{0:>3} {1:>16}'.format(8, 10 ** 8))
   
	print('{0:>3} {1:>16}'.format(9, 10 ** 9))
   
	print('{0:>3} {1:>16}'.format(10, 10 ** 10))


Dalam contoh di atas terdapat **{ }** yang berfungsi sebagai ***placeholder*** atau penempat **arguments**.

Argument secara default urutannya adalah **berurutan**. 




Gambar 5 :

![Output_String3](https://user-images.githubusercontent.com/56499371/68083028-a1ff0c80-fe56-11e9-86b8-67e757a2e50c.png)


Misalnya dalam contoh di atas, terdapat argument **"0"** dan **"10 ** **0"**** didalam **format(0, 10 ** 0)**, yang dipisah dengan tanda **","** (koma), yang berarti 

__"0"__ adalah argument  **pertama** dan  __"10**0"__ adalah argument ke **dua**.  Sedangkan angka **0** dan **1** di dalam ***placeholder***, merupakan urutan yang 

kita masukan. Misalnya ***placeholder*** pada urutan pertama yaitu "{**0**:>3}" dan kita ingin mengganti menjadi "**1**" maka yang akan dicetak di ***placeholder*** 

pertama adalah output dari "**10 ** 0**".

**Contoh kode :**

    

	print('{1:>3} {0:>16}'.format(0, 10 ** 0))



Selanjutnya : 

**Output yang didapat :**

Gambar 6:
![Output_String4](https://user-images.githubusercontent.com/56499371/68083030-a4f9fd00-fe56-11e9-815b-2aee2a9b317a.png)

Sedangkan untuk "**:>3**" digunakan untuk menentukan output di cetak pada urutan ke tiga. Urutan yang kosong akan menghasilkan output "**spasi**".



## Lab2


Didalam lab2 ini akan membahas tentang bagaimana cara memasukan cara untuk input, menghitung dan mengubah tipe data serta membuat format print yang akan dicetak ke 

output.


**Contoh kode :**

	a = input("masukan nilai a:"
         
	b = input("masukan nilau b:")
         
	print("variabel a =", a)
         
	print("variabel b =", b)
         
	print('hasil penggabungan {1} & {0} = %d'.format(a, b))
         
         
	
	a = int(a)
         
	b = int(b)
         
         
	
	print('hasil penjumlahan {1} & {0} = %d'.format(a, b)%(a + b))
         
	print('hasil pembagian {} & {} = %d'.format(a, b) % (a / b))
         

 **Output yang didapat :**
         
        

 ![output_lab](

Input dimasukan dengan cara menjalankan program terlebih dahulu, kemudian data dimasukan oleh user (Lihat angka 10 & 6 hijau) dengan diikuti keterangan berupa string 

"masukan nilai a:". Lalu input di cetak menggunakan fungsi "print()", disertai keterangan "hasil penggabungan" seperti berikut. Kode :
         
          

			
		 print('hasil penggabungan {1} & {0} = %d'.format(a, b))


Didalam Input dicetak kembali disertai dengan format baru menggunakan fungsi "format". Output dari print ini berbentuk tipe data string. Jadi bila kita menjumlahkan 

input "a" dan "b" dengan operator "+" maka output dari penjumlahan tersebut akan menghasilkan "106" (10 dan 6). Sedangkan "%d" yang seharusnya hanya dilakukan proses 

dan tidak di cetak ke output, menjadi tercetak kedalam bentuk string atau text (lihat hasil output di atas). Tetapi jika kita menggunakan tipe data, misalnya "/" maka 

akan terjadi error. Ini disebabkan karena tipe data yang berbentuk string atau text tidak bisa di jumlahkan dengan operator tersebut. Maka dari itu kita perlu 

mengkonversikan atau mengubah tipe data tersebut menjadi tipe data bersifat bilangan atau angka, misalnya integer atau float.
         
        


			 a = int(a)
		
         b = int(b)

Perintah di atas akan mengkonversikan tipe data sebelumnya ke bentuk tipe data integer. Dengan ini kita bisa menjumlahkan input sebagai angka.
         
    

					 print('hasil penjumlahan {1} & {0} = %d'.format(a, b)%(a + b))
         



Dilam perintah di atas digunakan untuk mencetak, menghitung dan memformat kembali output yang akan dihasilkan. "{1}" dan "{0}" adalah placeholder dan "%d" adalah 

perintah untuk mencetak output ke dalam bentuk desimal. Kita bisa mengubah "%d" menjadi, misalnya "%f", dan output yang akan di hasilkan akan dicetak dalam bentuk 

float.

	
