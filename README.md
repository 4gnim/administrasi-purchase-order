# Administrasi Purchase Order & Monitoring Penerimaan Barang

Proyek portofolio simulasi administrasi operasional menggunakan Microsoft Excel untuk pencatatan, pemeriksaan, monitoring penerimaan barang, dan pelaporan Purchase Order.

## Tujuan

Mensimulasikan alur kerja administrasi yang mencakup:

- Menjaga data Purchase Order tetap terstruktur.
- Menghitung jumlah barang yang masih outstanding.
- Mengukur persentase penerimaan.
- Membandingkan tanggal penerimaan aktual dengan tanggal yang diharapkan.
- Mengklasifikasikan status PO.
- Menyusun laporan monitoring operasional.

## Struktur proyek

```text
administrasi-purchase-order/
├── index.html
├── style.css
├── README.md
├── DEPLOY.md
└── screenshots/
    ├── raw-data.png
    ├── monitoring.png
    └── laporan.png
```

Tambahkan workbook Excel hasil proyek ke root repository sebagai:

`Administrasi_Purchase_Order.xlsx`

## Hasil utama

- Total Purchase Order: 18.000
- PO selesai: 15.801
- PO sebagian diterima: 1.326
- PO belum diterima: 467
- PO dibatalkan: 406
- Total quantity dipesan: 16.705.221
- Total quantity diterima: 15.288.825
- Outstanding quantity: 1.416.396
- Persentase penerimaan: 92%
- PO terlambat: 13.311

## Rumus Excel utama

```excel
=K2-L2
=IFERROR(L2/K2;0)
=IF(D2="";"";D2-C2)
=COUNTIF(...)
```

Rumus tersebut digunakan untuk menghitung outstanding quantity, receiving percentage, delivery variance, dan rekap status.

## Dataset

Proyek menggunakan **Inventory & Supply Chain Dataset v1.0.0** dari Analytics Engineering. Dataset tersebut merupakan **synthetic educational data** untuk pembelajaran dan pengujian, bukan data perusahaan nyata.

Lisensi: **CC BY 4.0**.

Sumber:
https://www.analyticsengineering.com/datasets/inventory-supply-chain

Sitasi:
Analytics Engineering. (2026). *Inventory & Supply Chain Dataset (Version 1.0.0)* [Data set].

## Catatan

Angka dan klasifikasi pada halaman ini mengikuti workbook hasil proyek. Jika workbook diperbarui, angka pada halaman dapat ikut diperbarui agar tetap konsisten.
