# -End-striyel-Yapay-Zeka-Asistan-
Genel Amaçlı Endüstriyel Yapay Zeka Asistanı
# 🏭 Endüstriyel Yapay Zeka Asistanı & RAG-Lite Analitik Platformu

Bu proje, üretim tesislerindeki makine loglarını, üretim adetlerini ve duruş/arıza kayıtlarını analiz ederek doğal dilde yanıt veren yapay zeka destekli bir asistan ve raporlama paneli sunar. Sistemin temel amacı; üretim verilerini anlamlandırmak, operasyonel verimliliği artırmak ve kestirimci bakım süreçleri için hızlı içgörüler oluşturmaktır.

## 🌟 Temel Özellikler

* **RAG-Lite Mimarisi:** Yerel veritabanından (SQL/Excel) çekilen verilerin filtrelenip dinamik bir veri bağlamı (context) olarak LLM'e (Büyük Dil Modeli) aktarılması.
* **Semantic Routing (Anlamsal Yönlendirme):** Kullanıcı niyetini (intent) deterministik olarak algılayan ve LLM halüsinasyonunu (hallucination) minimize eden özel kural tabanlı yönlendirme sistemi.
* **Kestirimci Bakım Çözüm Havuzu:** Sık yaşanan endüstriyel arızalar (pnömatik valf, sensör odağı, motor ısınması vb.) için kök neden analizine dayalı anlık tavsiye motoru.
* **Dinamik Veri Entegrasyonu:** SQL Server üzerinden canlı verilerin otomatik olarak çekilmesi ve DataFrame üzerinde işlenmesi.
* **Modern Kullanıcı Arayüzü:** Flask tabanlı, uzay temalı, animasyonlu ve interaktif sohbet paneli.

## 🛠️ Kullanılan Teknolojiler

* **Backend:** Python, Flask, SQLAlchemy, Pandas, NumPy
* **AI & LLM:** Llama 3.1 (Ollama üzerinden Localhost entegrasyonu), Özel Prompt Engineering
* **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
* **Veri Kaynakları:** MS SQL Server, Excel (`.xlsx`)

## ⚙️ Kurulum ve Çalıştırma Adımları

Projeyi kendi bilgisayarınızda yerel (local) olarak çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

### 1. Depoyu Klonlayın
\`\`\`bash
git clone https://github.com/KULLANICI_ADIN/endustriyel-ai-asistani.git
cd endustriyel-ai-asistani
\`\`\`

### 2. Gerekli Kütüphaneleri Yükleyin
Sisteminizde Python'un kurulu olduğundan emin olun ve bağımlılıkları yükleyin:
\`\`\`bash
pip install Flask pandas numpy sqlalchemy pyodbc requests
\`\`\`

### 3. Ollama ve Llama 3.1 Kurulumu
Proje, veri gizliliğini sağlamak adına tamamen yerel çalışan Llama 3.1 modelini kullanır.
* [Ollama'yı indirin ve kurun](https://ollama.com/)
* Terminali açıp modeli indirin ve başlatın:
\`\`\`bash
ollama run llama3.1
\`\`\`

### 4. Uygulamayı Başlatın
Ollama arka planda çalışırken yeni bir terminal sekmesi açın ve Flask sunucusunu başlatın:
\`\`\`bash
python app.py
\`\`\`
Uygulama `http://localhost:8080` adresinde çalışmaya başlayacaktır. Tarayıcınızdan bu adrese giderek asistanla etkileşime geçebilirsiniz.

## 📂 Proje Yapısı

* `app.py`: Sistemin kalbi. API rotaları, veri manipülasyonu, Semantic Router ve LLM haberleşmesini içerir.
* `uretim_tablosu.xlsx` & `ariza_tablosu.xlsx`: Sistemin analiz ettiği ve cevaplarını dayandırdığı deterministik veri setleri.
* `Raporlar/`: Geçmişe dönük pdf tabanlı sistem analizlerinin ve üretim kayıtlarının saklandığı dizin.

## 👨‍💻 Geliştirici
**Dilay Sümbül** - Elektrik-Elektronik Mühendisi & Yapay Zeka Geliştiricisi  
* [LinkedIn Profilim](linkedin.com/in/dilay-sümbül-3a1961254)
* [GitHub Profilim](https://github.com/dilaysumbul812-debug)
