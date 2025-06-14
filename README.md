<h1 align="center"> Retrieval-Augmented Generation with Gradio and Groq API Key</h1>
<p align="center"> Natural Language Processing Project</p>

<div align="center">

<img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54">

</div>

### Name : Fairah almira
### Tech Stack : Python, Gradio, LangChain, HuggingFace Embedding, FAISS vector store

---

### 1. Analysis about how the project works
- TODO

### 2. Analysis about how different every model works on Retrieval-Augmented Generation

```python
def get_llm():
    return ChatGroq(
        groq_api_key=GROQ_API_KEY,
        model_name="llama-3.3-70b-versatile", # Change the model in the code
        temperature=0.2
    )
```
- Model used : ```[llama-3.3-70b-versatile, deepseek-r1-distill-llama-70b, gemma2-9b-it]```

2.1 Analysis on ```llama-3.3-70b-versatile``` : 
“Dokumen ini membahas jenis-jenis antena BTS (macrocell, microcell, picocell, femtocell), arsitektur jaringan seluler, dan latar belakang perkembangan teknologi komunikasi seluler.”

- Jawaban sangat ringkas dan langsung ke inti.
- Menggunakan bahasa Indonesia, cocok untuk pengguna lokal.
- Hanya menyebut topik umum (jenis antena BTS, arsitektur jaringan, latar belakang teknologi).
- Kurang mendalam untuk konteks akademik atau dokumentasi panjang.
- Cocok digunakan untuk preview cepat atau aplikasi end-user sederhana.

2.2 Analysis on ```deepseek-r1-distill-llama-70b``` : 
"<details> <summary>Klik untuk melihat jawaban lengkap</summary> <pre> <think> Okay, so the user is asking about a file, but they didn't specify which one... </think> File ini tampaknya adalah dokumen yang membahas tentang jenis-jenis antena atau pemancar BTS (Base Transceiver Station) dan perkembangan arsitektur jaringan terkini dalam teknologi seluler. Berikut adalah ringkasan dari konten yang ada dalam file tersebut: 1. Jenis-Jenis Antena/Pemancar BTS: - Macrocell: Jangkauan beberapa kilometer, biasanya dipasang di menara tinggi untuk cakupan luas. - Microcell: Jangkauan ratusan meter, digunakan di area padat seperti mall atau jalan perkotaan. - Picocell: Jangkauan puluhan meter, dipasang di dalam gedung untuk memperbaiki sinyal indoor. - Femtocell: Jangkauan sangat terbatas, digunakan untuk memperkuat sinyal di rumah atau ruangan kecil. 2. Arsitektur Jaringan Terkini: - Membahas kebutuhan komunikasi bergerak, keterbatasan teknologi telepon tetap, inovasi radio & digitalisasi sinyal, serta peningkatan permintaan data. File ini kemungkinan besar merupakan bahan presentasi akademik oleh kelompok mahasiswa: - Muhammad Aditya Pratama (2022610024) - Sapta Eka Putra (2022610044) </pre> </details>"

- Memberikan jawaban paling lengkap, termasuk blok <think> yang menjelaskan reasoning internal model.
-Konten disusun secara terstruktur seperti penjelasan jenis antena BTS (Macrocell, Microcell, Picocell, Femtocell) serta latar belakang arsitektur jaringan dan faktor penggerak perkembangan teknologi seluler.
-Menyebut identitas mahasiswa sebagai pembuat file PDF.
-Cocok untuk laporan akademik, dokumentasi teknis, dan penulisan naratif mendalam.

2.3 Analysis on ```gemma2-9b-it``` : 
“This file appears to be a report or presentation about cellular network technology.
It includes:
Different types of antennas/transmitters used in BTS (Base Transceiver Station): Macrocell, Microcell, Picocell, and Femtocell.
Information about the current network architecture and its evolution.
A background section discussing the key factors driving the development of mobile technology.”

- Menyajikan informasi dengan gaya bullet point dalam bahasa Inggris.
- Fokus pada struktur dan isi dokumen (jenis antena, arsitektur jaringan, dan latar belakang teknologi).
- Tidak ada penyesuaian konteks lokal atau bahasa pengguna.
- Cocok untuk draft awal dokumen teknis atau integrasi dengan sistem analitik otomatis yang membutuhkan format cepat.

### 3. Analysis about how temperature works

```python
def get_llm():
    return ChatGroq(
        groq_api_key=GROQ_API_KEY,
        model_name="llama-3.3-70b-versatile",
        temperature=0.2 # Change the temperature value here and analzye
    )
```

3.1 Analysis on higher temperature 
- TODO

3.2 Analysis on lower temperature
- TODO

### 4. How to run the project

- Clone this repository with : 

```git
git clone https://github.com/arifian853/RAG_with_GroqAPI.git
```

- Copy the ```.env.example``` file and rename it to ```.env```

```
GROQ_API_KEY=your-groq-api-key
```

- Fill the ```GROQ_API_KEY``` with your Groq API Key, find it here : https://console.groq.com/keys

- TODO
- TODO
- TODO
- TODO
- TODO
- TODO
- TODO
