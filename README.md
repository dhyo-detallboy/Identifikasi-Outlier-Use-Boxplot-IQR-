# Identifikasi Outlier dengan Boxplot & IQR

Proyek ini merupakan percobaan untuk mengidentifikasi outlier dalam dataset menggunakan **Boxplot** dan **IQR** (Interquartile Range) dengan menggunakan **Jupyter Notebook**.

## Deskripsi
Proyek ini bertujuan untuk melakukan identifikasi outlier pada dataset yang berisi data tentang tinggi badan dan berat badan menggunakan dua metode statistik:
- **Boxplot** untuk visualisasi distribusi data.
- **IQR** (Interquartile Range) untuk mendeteksi nilai-nilai yang terletak jauh dari distribusi normal data.

## Dataset
Dataset yang digunakan dalam proyek ini adalah **height_weight.csv**, yang berisi informasi tentang tinggi badan (Height) dan berat badan (Weight) beberapa individu. 

### Contoh Data:
| ID  | Height | Weight |
| --- | ------ | ------ |
| 1   | 170    | 65     |
| 2   | 180    | 75     |
| 3   | 150    | 45     |
| 4   | 160    | 55     |
| 5   | 165    | 60     |
| 6   | 175    | 70     |
| 7   | 155    | 50     |
| 8   | 200    | 90     |
| 9   | 165    | 60     |
| 10  | 167    | 67     |
| 11  | 162    | 58     |
| 12  | 158    | 53     |
| 13  | 210    | 100    |
| 14  | 185    | 80     |
| 15  | 168    | 65     |

Dataset by Alif Dio A.

## Instalasi
Untuk menjalankan proyek ini, pastikan Anda sudah menginstal **Jupyter Notebook** dan dependensi berikut:

1. **Clone repositori ini**:
    ```bash
    git clone https://github.com/dhyo-detallboy/Identifikasi-Outlier-Use-Boxplot-IQR-.git
    ```

2. **Instal dependensi**:
    ```bash
    pip install -r requirements.txt
    ```
   (Jika tidak ada file `requirements.txt`, kamu bisa menginstal dependensi seperti `matplotlib`, `seaborn`, `pandas`, dan `numpy` secara manual)

## Penggunaan
Buka file Jupyter Notebook yang ada di repositori ini dan jalankan langkah-langkah berikut:

1. **Load dataset** – Impor data yang akan dianalisis.
2. **Visualisasikan dengan Boxplot** – Buat plot untuk melihat distribusi data.
3. **Hitung IQR** – Gunakan metode IQR untuk mendeteksi nilai outlier.
4. **Label outlier** – Tandai nilai yang terdeteksi sebagai outlier.

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Contoh cara load dan analisis data
df = pd.read_csv('height_weight.csv')
sns.boxplot(x=df['Height'])
