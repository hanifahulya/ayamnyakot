# Ayam Nyakot Customer Order & Admin Tracking

Web sederhana berbasis **Streamlit** untuk membantu UMKM Ayam Nyakot menerima pesanan online dan mengelola pesanan melalui dashboard admin.

## Mode Aplikasi

### 1. Pelanggan

Pelanggan dapat:

1. Melihat menu Ayam Nyakot
2. Memilih menu ayam geprek
3. Memilih rasa: Tidak Pedas atau Pedas
4. Memilih metode pesanan: diantar atau ambil sendiri
5. Mengisi data nama, nomor WhatsApp, dan alamat
6. Mengirim pesanan secara online
7. Mengecek status pesanan menggunakan Order ID dan nomor WhatsApp

### 2. Admin / Owner

Admin dapat:

1. Melihat dashboard ringkasan pesanan
2. Melihat pesanan online yang masuk
3. Menambah pesanan manual
4. Mengubah status pesanan
5. Mengubah ongkir
6. Mengubah estimasi pesanan
7. Mengecek status pembayaran ongkir
8. Export data ke CSV dan Excel

## Menu Produk

| Produk | Harga |
|---|---:|
| Ayam Geprek Tanpa Nasi | Rp10.000 |
| Ayam Geprek Pakai Nasi | Rp15.000 |

## PIN Admin

PIN default admin untuk demo:

```text
1234
```

PIN bisa diganti langsung di file `app.py` pada bagian login admin.

## Struktur Folder

```text
ayam_nyakot_streamlit_customer_admin/
│
├── app.py
├── requirements.txt
├── README.md
├── data/
│   └── ayam_nyakot_delivery.csv
└── .streamlit/
    └── config.toml
```

## Cara Menjalankan di Laptop

```bash
pip install -r requirements.txt
streamlit run app.py
```

## Cara Deploy ke Streamlit

1. Upload semua file ke GitHub.
2. Buka Streamlit Community Cloud.
3. Pilih repository GitHub.
4. Main file path: `app.py`
5. Klik deploy.

## Catatan Penyimpanan Data

Versi ini memakai file CSV lokal pada folder `data/`.
Untuk demo project kuliah dan prototipe, cara ini sudah cukup.
Untuk penggunaan nyata jangka panjang, gunakan database online seperti Google Sheets, Firebase, Supabase, atau PostgreSQL.