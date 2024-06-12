# Visualisasi Algoritma Bubble Sort

Proyek ini adalah program Java yang memvisualisasikan algoritma Bubble Sort. Program ini menampilkan proses pengurutan dengan grafik dinamis sehingga pengguna dapat melihat setiap langkah perbandingan dan pertukaran elemen secara real-time.

## Pendahuluan

Bubble Sort adalah algoritma pengurutan sederhana yang mengulang langkah-langkah berikut:
1. Membandingkan dua elemen yang berdekatan.
2. Menukar elemen jika mereka berada dalam urutan yang salah.
3. Mengulangi proses ini sampai daftar terurut.

## Alur Visualisasi Grafik

### 1. Grafik Awal
- Menampilkan bar yang tidak terurut sesuai dengan input awal dari pengguna.

### 2. Selama Proses Bubble Sort
- **Setiap Perbandingan dan Pertukaran**: Bar yang dibandingkan dan ditukar akan diperbarui dalam grafik.
- **Repaint**: Memperbarui seluruh grafik untuk mencerminkan posisi elemen terbaru setelah setiap pertukaran.
- **Delay**: Memberikan jeda waktu yang membuat visualisasi pergerakan bar terlihat oleh pengguna.

### 3. Grafik Akhir
- Menampilkan bar yang sudah diurutkan sesuai dengan jarak dari yang terkecil hingga terbesar.

## Langkah-langkah Visualisasi

1. **Awal**:
   - Daftar jarak yang tidak terurut: `[56, 12, 34, 9]`
   - Grafik menampilkan bar dengan panjang bervariasi sesuai dengan nilai jarak.

2. **Iterasi 1 (Pass 1)**:
   - Membandingkan dan menukar elemen yang perlu diurutkan.
   - Array berubah menjadi `[12, 34, 9, 56]`.

3. **Iterasi 2 (Pass 2)**:
   - Melanjutkan perbandingan dan pertukaran.
   - Array berubah menjadi `[12, 9, 34, 56]`.

4. **Iterasi 3 (Pass 3)**:
   - Lanjutkan sampai semua elemen berada pada urutan yang benar.
   - Array berubah menjadi `[9, 12, 34, 56]`.

5. **Iterasi 4 (Pass 4)**:
   - Tidak ada perubahan yang dilakukan karena array sudah terurut.

6. **Array Akhir**:
   - Daftar jarak yang terurut: `[9, 12, 34, 56]`

## Contoh Output dan Visualisasi

### Awal:
- Daftar tidak terurut: `[56, 12, 34, 9]`
- Grafik menampilkan bar-bar sesuai dengan nilai jarak.

### Iterasi 1:
- Membandingkan 56 dan 12 → Tukar
- Membandingkan 56 dan 34 → Tukar
- Membandingkan 56 dan 9 → Tukar
- Array: `[12, 34, 9, 56]`

### Iterasi 2:
- Membandingkan 12 dan 34 → Tidak Tukar
- Membandingkan 34 dan 9 → Tukar
- Membandingkan 34 dan 56 → Tidak Tukar
- Array: `[12, 9, 34, 56]`

### Iterasi 3:
- Membandingkan 12 dan 9 → Tukar
- Membandingkan 12 dan 34 → Tidak Tukar
- Membandingkan 34 dan 56 → Tidak Tukar
- Array: `[9, 12, 34, 56]`

### Iterasi 4:
- Membandingkan 9 dan 12 → Tidak Tukar
- Membandingkan 12 dan 34 → Tidak Tukar
- Membandingkan 34 dan 56 → Tidak Tukar
- Array: `[9, 12, 34, 56]`

### Grafik Akhir:
- Bar-bar terurut dari yang terpendek (jarak terkecil) hingga yang terpanjang (jarak terbesar).

## Cara Menjalankan Program

1. Pastikan Java Development Kit (JDK) terinstal di komputer Anda.
2. Clone repositori ini:
   ```bash
   git clone https://github.com/username/bubble-sort-visualization.git
3. Navigasikan ke direktori proyek:
   ```bash
   cd bubble-sort-visualization
4. Kompilasi program:
   ```bash
   javac BubbleSortVisualization.java
5. Jalankan program:
   ```bash
   java BubbleSortVisualization
