# titanic-exploratory-analysis

# 🚢 Titanic Dataset Investigation (Exploratory Data Analysis)

Repository ini berisi script Python untuk melakukan eksplorasi awal (exploratory data analysis / EDA) terhadap dataset Titanic. Analisis ini mencakup pemeriksaan struktur data, ringkasan statistik, pencarian duplikat dan nilai yang hilang, serta penanganannya.

## 📋 Pertanyaan Investigasi

Analisis ini menjawab beberapa pertanyaan dasar seputar data:
1. **Cek Data Awal**
   - Menampilkan data dengan `.head()`, `.tail()`, `.sample()`, dan `.info()`
   - Observasi awal dari struktur dan isi dataset

2. **Statistical Summary**
   - Analisis deskriptif menggunakan `.describe()`
   - Observasi berdasarkan nilai mean, min, max, dan persebaran data

3. **Pemeriksaan Duplikat**
   - Identifikasi baris duplikat
   - Penanganan dengan `.drop_duplicates()`

4. **Pemeriksaan Missing Values**
   - Cek nilai hilang dengan `.isnull().sum()`
   - Hitung persentase missing value
   - Penanganan: `dropna()` atau `fillna()` sesuai konteks

## 🛠 Library yang Digunakan

```python
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Konfigurasi tampilan
pd.set_option("display.max_columns", None)
pd.set_option("display.max_rows", None)
