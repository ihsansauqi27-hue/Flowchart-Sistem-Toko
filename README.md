```mermaid
graph TD
    A([Mulai: Pelanggan Tiba]) --> B[Pindai QR / Kartu Kredit]
    B --> C{Verifikasi Pembayaran}
    C -- Tidak Valid --> D[Akses Ditolak]
    C -- Valid --> F[Gerbang Terbuka & Masuk]
    F --> E[Kamera AI Buat Profil Pelacakan]
    E --> G[Ambil Barang dari Rak]
    G --> H[Kamera + Sensor Rak Cocokkan Data]
    H --> I[Barang Masuk Keranjang Virtual]
    I --> J{Kembalikan Barang ke Rak?}
    J -- Ya --> K[Barang Dihapus dari Keranjang]
    K --> L[Pelanggan Keluar Toko]
    J -- Tidak --> L
    L --> M[Sistem Hitung Total]
    M --> N[Tagih Biaya ke Kartu Kredit]
    N --> O[Perbarui Database Inventaris]
    O --> P[Kirim Struk Digital]
    P --> Q([Selesai])
