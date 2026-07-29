<img width="1024" height="1024" alt="jelly" src="https://github.com/user-attachments/assets/3e518e1e-a623-4186-be0c-29cfad72ef53" />RAG Tabanlı Akıllı Chatbot

Bu proje, yaz stajı sürecimde kurumsal ERP sistemlerindeki (özellikle SAP/HANA) iş süreçlerinin ve firmalara özel olarak tanımlanan 'Z'li işlem kodlarının çalışanlar tarafından daha hızlı, verimli ve hatasız kullanılabilmesi amacıyla tasarlanmıştır. Kurum içi bilgi birikimini dijitalleştiren bu sistem, geleneksel ve statik dokümantasyonlar yerine kullanıcıların doğal dilde sorular sorarak doğrudan sisteme özel yanıtlar alabildiği etkileşimli bir asistan sunmaktadır. Projenin en güçlü yönü, veri kaynaklarının (örneğin `kaynak.md` dosyası) ana mimariden tamamen izole edilmiş olması sayesinde son derece modüler ve "tak-çalıştır" bir esnekliğe sahip olmasıdır. Bu bağımsız yapı sayesinde uygulamanın sadece tek bir firmaya veya SAP sistemine özel kalması gerekmez; ihtiyacı olan herkes projeyi kendi ERP sistemlerine (Oracle, Microsoft Dynamics vb.), İK prosedürlerine veya farklı kurumsal yönergelerine kolayca entegre edebilir. Başka bir kullanım alanına uyarlamak için yapılması gereken tek şey, o kuruma ait özel verileri kaynak dizinine eklemektir; sistem yeni verileri otomatik olarak işleyerek chatbot'u saniyeler içinde istenilen firmaya veya alana özel bir uzmana dönüştürür..Spesifik veri setleri üzerinde Retrieval-Augmented Generation (RAG) mimarisi çalıştıran bağlam farkındalıklı bir chatbot uygulamasıdır. Doğal dil işleme (NLP) teknikleri ve LLM entegrasyonu kullanılarak, kullanıcının sorularına yalnızca sağlanan kaynak dosyalar üzerinden, doğruluğu teyit edilmiş ve halüsinasyondan arındırılmış yanıtlar üretmeyi hedefler.

RAG Mimari Entegrasyonu: Vektör arama işlemleriyle bağlama en uygun verilerin getirilmesi.
LLM Servis Yönetimi: Dil modeliyle optimize edilmiş iletişim ve istem (prompt) yönetimi. 
Otomatik Veri Dönüşümü: Yapılandırılmış Excel verilerinin LLM'in daha iyi analiz edebileceği Markdown formatına dönüştürülmesi.
Kaynak Doğrulama ve Güvenlik: Üretilen yanıtların kaynak metinlerle eşleşip eşleşmediğinin mantıksal kontrolü .


Teknolojiler ve Mimari
* Dil Modeli Entegrasyonu (LLM)
* Retrieval-Augmented Generation (RAG) Vektör Arama
* Python tabanlı Backend
* Kullanıcı Arayüzü (Frontend)

