<img width="1024" height="1024" alt="jelly" src="https://github.com/user-attachments/assets/3e518e1e-a623-4186-be0c-29cfad72ef53" />RAG Tabanlı Akıllı Chatbot

# 🤖 Kurumsal ERP Sistemleri için RAG Tabanlı Akıllı Chatbot

Bu proje, kurumsal ERP sistemlerindeki (özellikle SAP/HANA) karmaşık iş süreçlerinin ve kuruma özel tanımlanmış 'Z'li işlem kodlarının kullanıcılar tarafından hızlı, verimli ve hatasız bir şekilde kullanılabilmesi için tasarlanmış akıllı bir asistandır.

Geleneksel ve statik dokümantasyonları dijitalleştiren bu sistem, kullanıcıların doğal dilde sorular sorarak sistem kullanımına dair anında, teyit edilmiş ve halüsinasyondan arındırılmış yanıtlar almasını sağlar.

## ✨ Öne Çıkan Özellikler

*   **Modüler ve "Tak-Çalıştır" Mimari:** Sistemin bilgi kaynağı (ör. `kaynak.md`) ana mimariden tamamen izole edilmiştir. Bu sayede proje sadece belirli bir SAP sistemine bağımlı kalmaz; Oracle, Microsoft Dynamics veya farklı İK yönergeleri için sadece veri kaynak dizini değiştirilerek saniyeler içinde yeni bir alana entegre edilebilir.
*   **RAG (Retrieval-Augmented Generation) Entegrasyonu:** Vektör arama işlemleriyle bağlamın doğru bir şekilde kayıt altına alınması ve yalnızca sağlanan kurum içi kaynak dosyaları üzerinden yanıt üretilmesi sağlanır.
*   **Otomatik Veri Dönüşümü:** Yapılandırılmış kurumsal Excel verileri, dil modelinin (LLM) daha yüksek doğrulukla analiz edebileceği Markdown formatına otomatik olarak dönüştürülür.
*   **Kaynak Doğrulama ve Güvenlik:** LLM servis yönetimi ile optimize edilmiş istem (prompt) mühendisliği kullanılarak, üretilen yanıtların kaynak metinlerle birebir eşleşip eşleşmediği kontrol edilir.

## 🛠️ Teknolojiler ve Mimari

*   **Dil Modeli ve Çerçeve (LLM & Framework):** LangChain, Groq LLM
*   **Vektör Veritabanı ve Gömme (Embeddings):** ChromaDB / HuggingFace
*   **Arka Uç (Backend):** Python
*   **Kullanıcı Arayüzü (Frontend):** PyQt6 Desktop GUI
*   **Yaklaşım:** RAG (Retrieval-Augmented Generation), Doğal Dil İşleme (NLP)

## 🚀 Kurulum ve Çalıştırma

Projeyi kendi yerel ortamınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1. Repoyu klonlayın:
   ```bash
   git clone [https://github.com/meryep/rag-chatbot-project.git](https://github.com/meryep/rag-chatbot-project.git)
2. Kütüphaneleri Kurun
   pip install -r requirements.txt
   
4. .env dosyanızı oluşturun ve gerekli API anahtarlarınızı (örn. Groq API Key) ekleyin.

Kurumunuza özel verileri /data klasörüne yerleştirin.

Uygulamayı başlatın:

Bash
python main.py
