# Pratikum2-pertemuan6

# Latihan 1

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


# Latihan 2

<img width="544" height="218" alt="image" src="https://github.com/user-attachments/assets/a2e4a439-1343-4e3b-8823-d9c701c5150f" />

menggunakan konvigurasi :

    # program mengurutkan data
    # menerima input dari pengguna
    bilangan1 = int(input("masukkan bilangan ke-1: "))
    bilangan2 = int(input("masukkan bilangan ke-2: "))
    bilangan3 = int(input("masukkan bilangan ke-3: "))
    
    # menyimpan bilangan ke dalam list
    daftar_bilangan = [bilangan1, bilangan2, bilangan3]
    
    # mengurutkan list
    daftar_bilangan.sort()
    # menampilkan hasil
    print("urutan bilangan:", daftar_bilangan)

•	Untuk menerima input dari pengguna, kita dapat menggunakan fungsi input() di Python. Input akan disimpan sebagai string, jadi kita perlu mengubahnya menjadi tipe data integer (int) untuk dapat diurutkan secara numerik.

•	Untuk mengurutkan data, cara yang paling umum adalah dengan menyimpannya dalam sebuah list. List adalah struktur data yang dapat menyimpan banyak item dalam satu variabel.

•	Menggunakan metode sort() untuk list yang dapat mengurutkan item dalam list secara berurutan dari yang terkecil ke terbesar (ascending order).

•	Setelah list diurutkan, kita dapat mencetaknya ke layar menggunakan fungsi print().

•	Program di atas akan menghasilkan output yang di inginkan

yang dihasilkan :

<img width="683" height="148" alt="image" src="https://github.com/user-attachments/assets/2ff0ab8a-7a1d-4216-8d82-97715624aef4" />


# Latihan 1

<img width="774" height="133" alt="image" src="https://github.com/user-attachments/assets/bb2609b5-fc9f-4c9d-ae55-c8c744d1d930" />

    # menerima input dari pengguna
    bilangan1 = float(input("masukkan bilangan pertama: "))
    bilangan2 = float(input("masukkan bilangan kedua: "))
    bilangan3 = float(input("masukkan bilangan ketiga: "))
    bilangan4 = float(input("masukkan bilangan keempat: "))

    # menentukan bilangan terbesar dari dua bilangan pertama menggunakan statment if
    if bilangan1 > bilangan2:
        terbesar = bilangan1
    else:
        terbesar = bilangan2

    # menampilkan hasil
    print(f"bilangan terbesar dari bilangan pertama dan kedua adalah: {terbesar}")

•	Tujuan dari program ini adalah untuk menerima empat input bilangan dari pengguna dan kemudian menentukan bilangan terbesar dari dua bilangan pertama menggunakan pernyataan if.

•	Fungsi input() digunakan untuk meminta pengguna memasukkan bilangan. Karena bilangan bisa berupa desimal, gunakan float() untuk mengonversi input string menjadi tipe data float.

Gunakan pernyataan if untuk memeriksa apakah bilangan1 lebih besar dari bilangan2.

•	Jika bilangan1 > bilangan2, maka bilangan1 adalah yang terbesar.

•	Jika tidak (else), maka bilangan2 adalah yang terbesar.

•	Simpan hasil perbandingan ini dalam variabel baru, misalnya terbesar.

Cetak hasil yang disimpan dalam variabel terbesar untuk menunjukkan bilangan mana yang lebih besar.
Hasilnya seperti berikut :

<img width="706" height="166" alt="image" src="https://github.com/user-attachments/assets/fcdc8291-f72b-4a2a-af69-9747ac9ae481" />


# Latihan 2

<img width="536" height="286" alt="image" src="https://github.com/user-attachments/assets/e8e034bd-ee56-4247-ae23-775a85a4f679" />

    import random
    # meminta input dari pengguna untuk jumlah bilangan
    n = int(input("masukkan jumlah n: "))

    # menggunakan loop while untuk menghasilkan bilangan acak
    # sampai n bilangan yang kurang dari 0.5 ditemukan
    while n > 0:
        # menghasilkan bilangan acak antara 0.0 dan 1.0
        random_number = random.random()

        # memeriksa apakah bilangan acak kurang dari 0.5
        if random_number < 0.5:
            # menampilkan bilangan jika memenuhi syarat
            print(random_number)

            # mengurangi n karena satu bilangan sudah ditemukan
            n -= 1

•	Impor Modul: Mengimpor modul random untuk fungsi pembangkit bilangan acak.

•	Input Pengguna: Meminta pengguna untuk memasukkan jumlah bilangan yang akan diproses, yang disimpan dalam variabel n.

•	Perulangan: Melakukan perulangan while sebanyak n kali.

•	Pembangkitan Bilangan Acak: Di setiap perulangan, program menghasilkan satu bilangan acak antara 0.0 dan 1.0.

•	Kondisi dan Output: Memeriksa apakah bilangan acak tersebut kurang dari 0.5. Jika ya, bilangan tersebut akan dicetak ke layar.

•	Pembaruan Variabel: Mengurangi nilai n sebesar 1 di setiap iterasi perulangan hingga n mencapai 0.

Dan menghasilkan :

<img width="686" height="168" alt="image" src="https://github.com/user-attachments/assets/654c04c8-4a3a-49be-9138-f167e505cfbd" />



    


