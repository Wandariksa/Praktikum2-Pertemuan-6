<img width="429" height="220" alt="SOAL 1" src="https://github.com/user-attachments/assets/6a0a63b5-01bc-45da-a221-cf04636610ef" />

Pola yang diminta Adalah matriks angka berukuran 10x10.

•	Baris pertama (indeks 0) dimulai dari 0 dan setiap angka berikutnya bertambah 1. 

•	Baris kedua (indeks 1) dimulai dari 1 dan setiap angka berikutnya bertambah 1. 

•	Baris ke-i (indeks i) dimulai dari i. 

•	Angka di setiap sel pada baris i dan kolom j dapat dihitung dengan rumus: (i+j).
Menggunakan perulangan for yang bersarang (nested)

•	Perulangan luar akan mengontrol baris, dari 0-9

•	Perulangan dalam akan mengontrol kolom dari 0-9



for i in range(1, 10):

    # Perulangan dalam (inner loop) untuk kolom
    
    for j in range(1, 10):
    
        # Menghitung hasil perkalian
        
        hasil = i + j
        
        # Mencetak hasil dengan format rata kanan
        
        print(f"{hasil:>4}", end="")
    
    # Pindah ke baris baru setelah perulangan dalam selesai
    print()


•	for i in range(10): akan mengulangi blok kode sebanyak 10 kali, dengan i mengambil nilai 0, 1, 2, ..., 9. Ini mewakili baris.

•	for j in range(10): akan mengulangi blok kode sebanyak 10 kali, dengan j mengambil nilai 0, 1, 2, ..., 9. Ini mewakili kolom.

•	print(i + j, end=" ") akan mencetak hasil penjumlahan i dan j. Argumen end=" " digunakan agar setiap angka dicetak di baris yang sama dengan spasi sebagai pemisah.

•	print() akan mencetak baris baru setelah setiap baris selesai dicetak.

maka hasilnya :
<img width="540" height="235" alt="image" src="https://github.com/user-attachments/assets/5cc94f76-b6c1-4f3c-8e97-ac6213766549" />



