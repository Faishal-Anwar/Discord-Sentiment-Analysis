# Discord Sentiment Analysis (Ulasan Bahasa Indonesia)

## Deskripsi Proyek
Proyek ini bertujuan untuk membangun sistem **analisis sentimen otomatis** berdasarkan ulasan pengguna Discord berbahasa Indonesia. Sistem ini mengklasifikasikan pesan menjadi tiga kategori sentimen: **positif**, **negatif**, dan **netral**.

Proyek menggunakan pendekatan NLP (Natural Language Processing) dan Machine Learning dengan pipeline yang mencakup: pembersihan data teks, tokenisasi, stopword removal, stemming, visualisasi WordCloud, dan pelatihan model klasifikasi.

---

## Tujuan
Membantu dalam:
- Memahami persepsi dan kepuasan komunitas terhadap platform Discord.
- Mengidentifikasi potensi konflik atau feedback penting secara otomatis.
- Menyediakan dasar bagi sistem moderasi berbasis AI atau pemantauan sosial.

---

## Teknologi yang Digunakan

### 1. **Natural Language Processing (NLP)**
- Bahasa Indonesia: menggunakan pustaka **Sastrawi** untuk *stemming* dan *stopword removal*.
- Tokenisasi dengan **NLTK**.
- Pembersihan teks dengan regex dan transformasi lower-case.

### 2. **Visualisasi**
- **Seaborn & Matplotlib**: untuk visualisasi distribusi sentimen.
- **WordCloud**: untuk melihat kata-kata dominan pada tiap label sentimen.

### 3. **Model Klasifikasi**
- Pendekatan awal dengan **TF-IDF Vectorizer**.
- Evaluasi menggunakan akurasi, classification report, dan confusion matrix.
- Model yang diuji termasuk:
  - Logistic Regression
  - Naive Bayes
  - Random Forest (opsional tergantung isi notebook lengkap)

---

## Hasil Sementara

![image](https://github.com/user-attachments/assets/fbdd5285-22c3-4815-a7ec-74d3dedff7c6)

![image](https://github.com/user-attachments/assets/d124ddbb-4af1-4124-a64e-0409b401a6b9)
![image](https://github.com/user-attachments/assets/6a8ba73b-5a7c-447a-8591-aa79e28a5c86)

- Dataset dibersihkan dari duplikat dan null value.
- Model klasifikasi awal menunjukkan hasil yang menjanjikan.
- Distribusi sentimen dan WordCloud memperlihatkan insight awal terhadap kata-kata paling sering muncul di tiap label.

---

## 🛠️ Cara Menjalankan Proyek Ini

### 1. Clone Repository
```bash
git clone https://github.com/your-username/Discord-Sentiment-Analysis.git
cd Discord-Sentiment-Analysis

#### 2. Buat Virtual Environment
Sangat disarankan untuk menggunakan virtual environment agar dependensi proyek tidak bercampur dengan instalasi Python global Anda.
```bash
virtualenv venv
```

#### 3. Aktifkan Virtual Environment
```bash
venv\Scripts\activate
```
macOS/Linux:
```bash
source venv/bin/activate
```
Setelah aktif, nama environment (venv) akan muncul di awal baris terminal Anda.

#### 4. Instal Dependensi
Instal semua pustaka Python yang dibutuhkan yang tercantum dalam file requirements.txt.
```bash
pip install -r requirements.txt
```

#### 5. Jalankan Jupyter Notebook
Setelah semua dependensi terinstal, jalankan server Jupyter Notebook.
```bash
jupyter notebook
```
Perintah ini akan membuka tab baru di browser web Anda. Dari sana, navigasikan dan buka file notebook.ipynb untuk menjalankan kode.
