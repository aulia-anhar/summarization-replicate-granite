# Granite Summarization via Replicate API

Proyek ini berfokus pada **teks summarization (perangkum teks)** menggunakan model **Granite (ibm-granite/granite-3.3-8b-instruct)** yang dijalankan melalui **Replicate API**.  
Notebook ini juga mencakup evaluasi performa model menggunakan **ROUGE score** pada dataset **CNN/DailyMail**.

---

## 📌 Fitur Utama
- Integrasi model Granite via **Replicate API**.
- Eksperimen summarization pada dataset **CNN/DailyMail (3.0.0)**.
- **Exploratory Data Analysis (EDA)**: distribusi panjang artikel, wordcloud.
- Evaluasi performa model menggunakan **ROUGE (ROUGE-1, ROUGE-2, ROUGE-L, ROUGE-Lsum)**.
- Analisis hasil evaluasi dengan bantuan Granite.

---

## 🚀 Instalasi
Clone repository ini:
```bash
git clone https://github.com/username/granite-summarization.git
cd granite-summarization
````

Instal dependensi yang diperlukan:

Daftar library utama:

* `replicate`
* `langchain_community`
* `datasets`
* `evaluate`
* `rouge_score`
* `matplotlib`, `seaborn`, `wordcloud`

---

## 🔑 API Token

Sebelum menjalankan notebook, pastikan Anda sudah memiliki **Replicate API Token**:

```python
import os
os.environ["REPLICATE_API_TOKEN"] = "your_api_token_here"
```

---

## 📊 Dataset

Proyek ini menggunakan **CNN/DailyMail**:

* Source: [HuggingFace Dataset](https://huggingface.co/datasets/cnn_dailymail)

Subset data yang digunakan:

* Train sample: 50 artikel
* Validation sample: 20 artikel

---

## 📓 Notebook

Notebook utama:

* `Summarization_Granite_via_ReplicateAPI.ipynb`

Alur eksperimen:

1. Setup environment & API token
2. Load dataset CNN/DailyMail
3. Exploratory Data Analysis (EDA)
4. Summarization dengan Granite
5. Evaluasi dengan ROUGE
6. Analisis & kesimpulan

---

## 📈 Hasil Sementara

* Granite berhasil menghasilkan ringkasan artikel dengan kualitas yang cukup baik.
* Evaluasi menggunakan ROUGE menunjukkan bahwa performa Granite mendekati ringkasan referensi, meskipun masih ada ruang untuk perbaikan.

---

## 🤝 Kontribusi

Pull request dan masukan sangat diterima!
Untuk diskusi lebih lanjut, silakan buka *issue* di repository ini.

---

