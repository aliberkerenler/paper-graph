# AKADEMİK İŞBİRLİĞİ AĞ ANALİZİ

## 👥 Proje Sahipleri
* Ömer Faruk Toycu (@omertoycu)
* Ali Berke Erenler (@aliberkerenler)

---

## 🎯 Proje Amacı
Bu proje, akademik yayın verilerinden yazar işbirlikleri ağını analiz etmek ve görselleştirmek için tasarlanmış bir Python/Flask tabanlı web uygulamasıdır. Uygulama, yazarlar arası bağlantıları çıkarır, ağ yapısını oluşturur ve çeşitli algoritmalarla analiz sonuçlarını sunar.

## 🛠️ Teknolojiler ve Kütüphaneler
* **Dil:** Python
* **Web Çerçevesi:** [Flask](https://flask.palletsprojects.com/) (Web arayüzü ve routing için)
* **Veri İşleme:** `pandas` (Excel/CSV verisi okuma için)
* **Ağ Görselleştirme:** [PyVis](https://pyvis.readthedocs.io) (Etkileşimli ağ grafiği oluşturma için)
* **Algoritmalar:** BFS, Dijkstra, İkili Arama Ağacı (BST).

---

## ✨ Temel Analizler
Uygulama, akademik işbirliği ağını analiz etmek için aşağıdaki temel işlevleri sunar:

| İşlev | Uygulanan Algoritma/Metot | Açıklama |
| :--- | :--- | :--- |
| **En Kısa Yol (A-B)** | BFS (Genişlik Öncelikli Arama) | İki yazar arasındaki en kısa işbirliği mesafesini bulur ve grafikte vurgular. |
| **Düğüm Ağırlıkları** | `calculate_node_weights` | Belirli bir yazarla işbirliği yapan yazarları ve bu yazarların toplam makale sayılarını hesaplar. |
| **BST Oluşturma** | `BinarySearchTree` Sınıfı | Yazarlar listesinden bir İkili Arama Ağacı oluşturur ve görselleştirir (İsteğe bağlı düğüm silme içerir). |
| **Tüm Kısa Yollar** | Dijkstra Algoritması | Belirli bir yazardan diğer tüm yazarlara olan en kısa yolları hesaplar. |
| **İşbirlikçi Sayısı** | Graf analizi | Seçilen yazarın işbirliği yaptığı farklı yazar sayısını hesaplar. |
| **En Çok İşbirliği Yapan Yazar**| `find_most_collaborative_author` | Ağdaki en çok ortak makale sayısına sahip yazarı belirler. **Sonuç:** Rajeev Kumar, 344 işbirliği. |
| **En Uzun Yol** | Özyinelemeli Graf Arama | Belirli bir yazar düğümünden başlayan en uzun yolu bulur ve görselleştirir. |

---

## 🚀 Çalıştırma Talimatları
1. **Gereklilikleri Kurun:** Projeyi çalıştırmadan önce `flask`, `pandas`, `pyvis` gibi kütüphanelerin yüklü olduğundan emin olun.
2. **Uygulamayı Başlatın:** Python ortamınızda `Paper Graph.py` dosyasını çalıştırın.
3. **Erişim:** Tarayıcınızda `http://127.0.0.1:5000/` adresine gidin.
4. **Veri Yükleme:** Arayüzdeki formu kullanarak akademik verileri içeren Excel/CSV dosyanızı yükleyin.
5. **Analiz:** Yükleme sonrası açılan sayfada, sol menüdeki butonlar aracılığıyla istediğiniz ağ analizini başlatın. Görselleştirmeler yeni bir sekmede açılır.
