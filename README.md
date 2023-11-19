## Fragile-Watermarking

Alat ini mengimplementasikan Fragile Watermarking menggunakan metode Least Significant Bit (LSB). Fragile Watermarking adalah teknik yang memasukkan watermark yang sensitif ke dalam gambar, memungkinkan ekstraksi dan verifikasi integritas gambar kemudian.

### Penggunaan

1. **Menyisipkan Fragile-Watermarking:**
   Untuk menyematkan fragile watermarking ke dalam gambar, jalankan perintah berikut di terminal:
   ```bash
   python watermark-fragile.py <path_gambar_asli> <path_gambar_watermark> <path_output>
   ```
   - `<path_gambar_asli>`: Path ke gambar asli.
   - `<path_gambar_watermark>`: Path ke gambar watermark.
   - `<path_output>`: Path untuk menyimpan gambar dengan watermark.

2. **Mengekstrak Fragile-Watermarking:**
   Untuk mengekstrak fragile watermarking dari gambar, jalankan perintah berikut:
   ```bash
   python watermark-fragile.py <path_gambar_dengan_watermark> <path_output_watermark>
   ```
   - `<path_gambar_dengan_watermark>`: Path ke gambar dengan watermark.
   - `<path_output_watermark>`: Path untuk menyimpan watermark yang diekstrak.

### Fitur Fragile Watermarking

- **Enkripsi:** Alat ini menggunakan algoritma enkripsi sederhana untuk meningkatkan keamanan watermark.
- **Pengacakan:** Pengacakan piksel digunakan untuk meningkatkan ketangguhan dan keacak-acakan penyisipan watermark.
- **Analisis PSNR:** Setelah penyisipan, alat memberikan analisis Peak Signal-to-Noise Ratio (PSNR) untuk mengevaluasi kualitas gambar dengan watermark.

### Petunjuk

1. Jalankan skrip dan pilih operasi yang diinginkan (Sisipkan atau Ekstrak).
2. Sediakan masukan yang diperlukan, seperti path ke gambar dan kunci enkripsi.
3. Lihat hasil dan analisis PSNR untuk watermark yang disisipkan.

### Contoh Penggunaan

1. **Menyisipkan fragile watermarking:**
   ```bash
   python watermark-fragile.py gambar_asli.png watermark.png gambar_dengan_watermark.png
   ```
   
2. **Mengekstrak fragile watermarking:**
   ```bash
   python watermark-fragile.py gambar_dengan_watermark.png watermark_diekstrak.png
   ```

### Catatan

- Pastikan bahwa Python Imaging Library (PIL) terinstal sebelum menjalankan skrip.
- Kunci enkripsi sangat penting untuk penyisipan dan ekstraksi, jadi simpan dengan aman.

### Tampilan Program
1. **Menu Utama**

   ![image](https://github.com/raldyachmad/Fragile-Watermarking/assets/87338157/7d5321ee-2f0c-44a0-87b1-7f1a89b1a632)

2. **Menu Insert**

   ![image](https://github.com/raldyachmad/Fragile-Watermarking/assets/87338157/46b68fb5-951d-4d2d-94be-3c96afbb79e0)

3. **Menu Extract**

   ![image](https://github.com/raldyachmad/Fragile-Watermarking/assets/87338157/4bea3a4f-95fa-4d5b-9cf3-6f7df7c52fce)
