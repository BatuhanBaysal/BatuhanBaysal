<div align="center">
  <h1>👋 Batuhan Baysal</h1>
  <h3>Software Engineer | Java, Spring Boot & Distributed Systems Specialist</h3>

  <p align="center">
    Veri bütünlüğü, sistem dayanıklılığı (resilience) ve yüksek erişilebilirlik odaklı, 
    kurumsal standartlarda backend mimarileri geliştiren bir yazılım mühendisiyim.
  </p>

  <div align="center">
    <img src="https://img.shields.io/badge/Project%20Impact-1.1k+%20Clones-brightgreen?style=for-the-badge&logo=github" alt="Impact">
    <img src="https://img.shields.io/badge/Architecture-Distributed%20Microservices-blue?style=for-the-badge" alt="Architecture">
    <img src="https://img.shields.io/badge/Testing-Coverage%20100%25-blueviolet?style=for-the-badge" alt="Testing">
    <img src="https://img.shields.io/badge/Education-B.S.%20Computer%20Engineering-red?style=for-the-badge" alt="Education">
  </div>
</div>

---

## 🏗️ Mimari Yaklaşım & Mühendislik Disiplini

Projelerimi geliştirirken "çalışan kod"un ötesine geçerek, endüstriyel standartlarda (Enterprise-ready) sistemler inşa etmeye odaklanırım:

1. **Security & Identity Management:** Güvenliği merkezi bir katman olarak kurgularım. **Keycloak (OIDC/OAuth2)** ile IAM altyapısı oluşturuyor; **JWT, RBAC** ve **Resource Ownership** kontrolleriyle uçtan uca koruma sağlıyorum.
2. **Reliability & Event-Driven Design:** Dağıtık mimarilerde **RabbitMQ** ile asenkron iletişim kurguluyor, **Resilience4j** (Circuit Breaker, Rate Limiter) kullanarak sistemin cascade failure (zincirleme çökme) risklerini yönetiyorum.
3. **LGTM Stack Observability:** "Gözlemlenemeyen sistem, kontrol edilemeyen sistemdir." **Grafana Loki** (Logging), **Prometheus** (Metrics) ve **Zipkin/Tempo** (Tracing) ile sistemin runtime sağlığını tam şeffaflıkla izliyorum.

---

## 🏛️ Amiral Gemisi Projem: Secure Banking Core
Finansal veri bütünlüğü ve yüksek concurrency (eşzamanlılık) problemlerine çözüm olarak tasarlanmış kurumsal bir backend motorudur.

### 🚧 Teknik Zorluklar & Mühendislik Çözümleri

* **Zorluk: Deadlock (Karşılıklı Kilitlenme) Algoritması**
    * **Problem:** İki kullanıcının eşzamanlı olarak birbirine transfer başlatması durumunda oluşan dairesel beklemeyi (circular wait) çözmek.
    * **Çözüm:** **Alphabetical Resource Ordering** stratejisini uyguladım. Kaynakları alfabetik IBAN sırasına göre kilitleyerek deadlock olasılığını mimari seviyede elimine ettim.

* **Zorluk: Race Condition & Data Consistency**
    * **Problem:** Yüksek trafikli para transferlerinde "Double Spending" riskini önlemek.
    * **Çözüm:** **Pessimistic Write Locking** ve **Transaction Isolation** seviyelerini optimize ederek bakiye operasyonlarını atomik hale getirdim.

* **Zorluk: Infrastructure Synchronization**
    * **Problem:** Veritabanı şema değişikliklerinin farklı ortamlarda manuel yönetiminden doğan tutarsızlıklar.
    * **Çözüm:** **Liquibase** ile "Migration-based" şema yönetimi kurguladım ve CI/CD süreçlerini otomatize ettim.

---

## 🛠️ Yetkinlik Matrisi & Stratejik Kararlar

| Katman | Teknoloji | Mühendislik Gerekçesi (Why?) |
| :--- | :--- | :--- |
| **Identity** | **Keycloak & OAuth2** | Kimlik yönetimini servis kodundan ayırmak ve profesyonel bir IAM (Identity Access Management) çözümü sunmak için. |
| **Observability** | **Loki, Prometheus, Tempo** | Log, Metrik ve Trace verilerini korele ederek hata tespit süresini (MTTR) minimize etmek için. |
| **Persistence** | **PostgreSQL & Redis** | İlişkisel veri tutarlılığı için PostgreSQL; performans darboğazlarını aşmak adına Redis caching katmanı için. |
| **Messaging** | **RabbitMQ** | Servisler arası sıkı bağımlılığı (Tight Coupling) kırmak ve hata toleranslı event-driven iş akışları için. |
| **Resilience** | **Resilience4j** | Dağıtık sistemlerde ağ gecikmeleri veya servis kesintilerine karşı sistem dayanıklılığını korumak için. |
| **Quality Gate** | **SonarQube & JUnit 5** | Statik kod analizi ve %100 test coverage ile teknik borçlanmayı (Technical Debt) önlemek için. |

---

## 🚀 Diğer Stratejik Projeler

* **[Spring Cloud Observability](https://github.com/BatuhanBaysal/spring-cloud-observable-microservices):** Dağıtık sistemlerde hata takibi (distributed tracing) üzerine LGTM Stack kullanarak kurguladığım monitoring altyapısı.
* **[Secure Note App (Full-Stack)](https://github.com/BatuhanBaysal/fullstack-secure-noteapp-spring-react):** Spring Security ve React.js entegrasyonu ile JWT tabanlı stateless güvenlik ve RBAC modellemesi.
* **[Auth & Notification Microservice Stack](https://github.com/BatuhanBaysal/auth-notification-microservice-stack):** Redis tabanlı caching ve RabbitMQ ile asenkron mesajlaşma üzerinden servisler arası iletişimi (decoupling) optimize ettiğim mikroservis çalışması.
* **[AWS Parameter Store Integration](https://github.com/BatuhanBaysal/aws-parameter-store-spring-boot-crud):** Konfigürasyon yönetimini bulut ortamına (AWS) taşıyarak "Externalized Configuration" prensibini uyguladığım proje.

---

## 📈 Engineering Stats
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=BatuhanBaysal&show_icons=true&theme=dark&title_color=6DB33F&text_color=ffffff&hide_border=true" />
</div>

---

## 🤝 İletişim
* **Profesyonel Yaklaşım:** Sadece kod yazmaya değil, ölçeklenebilir ve sürdürülebilir mimari kararlar almaya odaklanırım.
* **İletişim:** [LinkedIn](https://www.linkedin.com/in/batuhan-baysal/) | [Email](mailto:batuhanbaysal3@gmail.com)

<div align="center">
  <img src="https://img.shields.io/badge/Main%20Stack-Java%20%26%20Spring-orange?style=for-the-badge&logo=java" />
</div>
