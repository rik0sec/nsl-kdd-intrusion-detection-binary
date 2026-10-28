# Dataset NSL-KDD

Dataset **tidak disertakan** di repository ini. Unduh sendiri lalu letakkan di folder ini.

## Cara mengunduh

1. Buka halaman dataset di Kaggle: <https://www.kaggle.com/datasets/hassan06/nslkdd>
2. Klik **Download** (perlu login Kaggle) lalu ekstrak arsipnya.
3. Salin **dua file** berikut ke folder `data/`:

```
data/
├── README.md
├── KDDTrain+.txt
└── KDDTest+.txt
```

Atau lewat Kaggle CLI:

```bash
kaggle datasets download -d hassan06/nslkdd -p data/ --unzip
```

## Tentang file

| File | Jumlah baris | Keterangan |
|------|-------------:|------------|
| `KDDTrain+.txt` | 125.973 | Data latih: 41 fitur + `label` + `difficulty` (tanpa header). |
| `KDDTest+.txt` | 22.544 | Data uji. Memuat 17 jenis serangan yang tidak ada di data latih. |

Nama kolom didefinisikan langsung di dalam notebook karena file tidak memiliki baris header.
