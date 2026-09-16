# Pertemuan 03 Seleksi Python

Nama: Nuril Ilmy  
NIM: 2225250066  
Kelas: 3E

## Tujuan

Mempelajari seleksi dalam Python menggunakan:
- if
- if-else
- kondisi majemuk (and, or, not)
- nested if

Selain itu, melakukan pengujian program berdasarkan test case dan mengunggah hasil pekerjaan ke GitHub.

## Struktur Folder

```text
pertemuan-03-seleksi-2225250066/
│
├── README.md
├── .gitignore
│
├── latihan/
│   ├── 01_genap_ganjil.py
│   ├── 02_bandingkan_dua_bilangan.py
│   ├── 03_kelulusan_bersyarat.py
│   └── 04_jenis_segitiga.py
│
└── tugas/
    └── analisis_persamaan_kuadrat.py
```

## Latihan

### 1. Genap atau Ganjil

Program menerima satu bilangan bulat kemudian menentukan apakah bilangan tersebut termasuk bilangan genap atau ganjil.

Kondisi yang digunakan:

```python
bilangan % 2 == 0
```

Jika kondisi benar, bilangan dinyatakan genap. Jika kondisi salah, bilangan dinyatakan ganjil.

### 2. Membandingkan Dua Bilangan

Program menggunakan nested if untuk membandingkan dua bilangan.

Hasil yang dapat ditampilkan:
- Bilangan pertama lebih besar
- Bilangan pertama lebih kecil
- Kedua bilangan sama

### 3. Kelulusan Bersyarat

Mahasiswa dinyatakan lulus jika memenuhi dua kondisi:

```text
nilai >= 60
dan
kehadiran >= 80
```

Operator logika yang digunakan adalah `and`.

### 4. Jenis Segitiga

Program menerima tiga panjang sisi dan terlebih dahulu memeriksa apakah ketiga sisi dapat membentuk segitiga.

Jika valid, program menentukan jenis segitiga:
- Segitiga sama sisi
- Segitiga sama kaki
- Segitiga sembarang

Program menggunakan kondisi majemuk dan nested if.

## Tugas 2: Analisis Persamaan Kuadrat

Program menganalisis persamaan:

```text
ax² + bx + c = 0
```

Program menerima nilai koefisien `a`, `b`, dan `c`.

Diskriminan dihitung menggunakan rumus:

```text
D = b² - 4ac
```

### Algoritma

1. Memasukkan nilai `a`, `b`, dan `c`.
2. Memeriksa apakah `a == 0`.
3. Jika `a == 0`, program menampilkan bahwa input bukan persamaan kuadrat.
4. Jika `a != 0`, menghitung diskriminan:

   ```text
   D = b² - 4ac
   ```

5. Jika `D > 0`, program menghitung dan menampilkan dua akar real berbeda.
6. Jika `D == 0`, program menghitung dan menampilkan satu akar real kembar.
7. Jika `D < 0`, program menampilkan bahwa tidak ada akar real.

## Cara Menjalankan

Jalankan program menggunakan Python melalui terminal VS Code.

Contoh untuk menjalankan tugas:

```bash
python tugas/analisis_persamaan_kuadrat.py
```

Untuk menjalankan latihan:

```bash
python latihan/01_genap_ganjil.py
python latihan/02_bandingkan_dua_bilangan.py
python latihan/03_kelulusan_bersyarat.py
python latihan/04_jenis_segitiga.py
```

## Hasil Pengujian

### Latihan 1

| Input | Hasil yang Diharapkan |
|---|---|
| 8 | Genap |
| 13 | Ganjil |
| 0 | Genap |
| -7 | Ganjil |

### Latihan 2

| Input | Hasil yang Diharapkan |
|---|---|
| (7, 4) | Bilangan pertama lebih besar |
| (2, 9) | Bilangan pertama lebih kecil |
| (5, 5) | Kedua bilangan sama |
| (-3, -8) | Bilangan pertama lebih besar |

### Latihan 3

| Nilai | Kehadiran | Hasil |
|---:|---:|---|
| 75 | 90 | Lulus |
| 59 | 90 | Belum lulus |
| 75 | 79 | Belum lulus |
| 60 | 80 | Lulus |

### Latihan 4

| Sisi a | Sisi b | Sisi c | Hasil |
|---:|---:|---:|---|
| 3 | 3 | 3 | Sama sisi |
| 5 | 5 | 8 | Sama kaki |
| 3 | 4 | 5 | Sembarang |
| 1 | 2 | 3 | Tidak membentuk segitiga |

### Tugas 2

| a | b | c | Diskriminan | Hasil |
|---:|---:|---:|---:|---|
| 1 | -5 | 6 | 1 | Dua akar real: 3 dan 2 |
| 1 | 2 | 1 | 0 | Akar kembar: -1 |
| 1 | 0 | 1 | -4 | Tidak ada akar real |
| 0 | 2 | 3 | - | Bukan persamaan kuadrat |

## Refleksi

Pada latihan seleksi Python, saya memahami bahwa pemilihan operator kondisi harus disesuaikan dengan aturan yang diberikan. Kesalahan yang perlu diperhatikan adalah penggunaan operator `>` dan `>=`, terutama pada nilai batas.

Saya juga memahami bahwa nested if digunakan ketika keputusan kedua bergantung pada hasil keputusan pertama.

Pengujian dengan beberapa test case, termasuk nilai batas, membantu memastikan setiap cabang program berjalan sesuai dengan kondisi yang ditentukan.

## Git dan GitHub

Perubahan program direkam menggunakan commit Git dan dikirim ke repositori GitHub menggunakan perintah:

```bash
git add .
git commit -m "feat: menyelesaikan latihan seleksi pertemuan 03"
git push
```