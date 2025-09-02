# Meringkas dan Mengklasifikasikan Keluhan Finansial Konsumen untuk Meningkatkan Layanan dan Regulasi Menggunakan IBM Granite

## 📌 Project Overview
Keluhan konsumen di sektor finansial terus meningkat setiap tahun, mencakup produk perbankan, kartu kredit, hipotek, dan layanan keuangan lainnya. 
Namun, volume data keluhan yang sangat besar menyulitkan perusahaan maupun regulator untuk memahami pola masalah utama.  
Proyek ini bertujuan untuk **mengklasifikasikan** keluhan berdasarkan jenis produk/isu dan **meringkas** temuan utama dengan bantuan IBM Granite, sehingga dapat menghasilkan wawasan yang actionable untuk meningkatkan layanan dan mendukung kebijakan regulasi.

## 🎯 Objective
- Mengklasifikasikan keluhan finansial konsumen berdasarkan kategori produk.
- Meringkas pola keluhan untuk memberikan insight yang bermakna.
- Menyediakan rekomendasi konkret bagi perusahaan dan regulator.
- Mendemonstrasikan penggunaan AI (IBM Granite) untuk data analytics, classification, dan summarization.

## 📂 Dataset
- **Sumber**: [Consumer Complaint Database](https://www.kaggle.com/datasets/selener/consumer-complaint-database)
- **Jumlah Data**: >3 juta keluhan sejak 2011
- **Fitur utama**:  
  - `Date received`  
  - `Product` (misal: Credit card, Bank account, Mortgage)  
  - `Issue` (masalah spesifik, misal: billing, interest, fraud)  
  - `Consumer complaint narrative` (teks keluhan)  
  - `Company` (bank/fintech terkait)

## 🔎 Analysis Process
1. **Data Cleaning**  
   - Hapus duplikasi & missing value.  
   - Normalisasi teks (lowercasing, stopword removal).  

2. **Classification**  
   - Target: kolom `Product` & `Issue`.  
   - Model baseline: Logistic Regression / Random Forest.  
   - Model LLM: IBM Granite untuk zero/few-shot classification.

3. **Summarization**  
   - Input: `Consumer complaint narrative` per produk/perusahaan.  
   - Output: ringkasan keluhan dominan (3–5 kalimat).  
   - IBM Granite digunakan untuk abstractive summarization.

4. **Visualization**  
   - Tren keluhan per tahun.  
   - Distribusi produk dengan keluhan terbanyak.  
   - Word cloud kata kunci per kategori.

## 💡 Insight & Findings
- Keluhan terbanyak tahun 2022 terjadi pada **kartu kredit**, mayoritas terkait **biaya tersembunyi & bunga**.  
- **Bank X** dan **Bank Y** mendominasi jumlah keluhan kartu kredit sejak 2019.  
- Keluhan terkait **pinjaman mahasiswa** melonjak signifikan pada 2021.  

## ✅ Conclusion & Recommendations
- **Untuk perusahaan finansial**: tingkatkan transparansi biaya, perbaiki proses penagihan.  
- **Untuk regulator**: awasi perusahaan dengan keluhan berulang; buat kebijakan perlindungan bunga pinjaman.  
- **Untuk konsumen**: perlu edukasi literasi finansial agar memahami hak & kewajiban.

## 🤖 AI Support Explanation
- **IBM Granite** digunakan untuk:  
  - *Classification*: mengelompokkan narasi keluhan ke dalam kategori produk/isu.  
  - *Summarization*: menghasilkan ringkasan naratif dari kumpulan keluhan.  
- AI mempercepat analisis dengan mengolah ribuan keluhan menjadi insight yang lebih mudah dipahami.

## 📎 Repository Content
- `notebook.ipynb` → Google Colab Notebook untuk preprocessing, classification, dan visualisasi.  
- `data/` → folder dataset (raw & processed).  
- `README.md` → dokumentasi proyek.  
- `presentation.pdf` → slide presentasi.  

---
