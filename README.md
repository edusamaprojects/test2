# Edusama AFS (Accommodation For Students)

## Projenin Amacı ve Hedefi
Bu proje, Türkiye'den Japonya'ya eğitim amacıyla giden öğrencilerin konaklama ihtiyaçlarını organize etmek, yönetmek ve sistematik şekilde takip edebilmek amacıyla geliştirilmiştir. Edusama AFS, konaklama teminiyle sınırlı kalmayıp konaklama birimlerinin durumu, kullanılan demirbaşlar, ödeme takibi ve muhasebe süreçlerini de bütüncül biçimde ele alarak kurum içi operasyonları kolaylaştırmayı hedefler.

## Hedef Kitle
- Japonya'da eğitim almak isteyen öğrenciler
- Edusama bünyesindeki operasyon yöneticileri
- Muhasebe ve kira takibini yapan personeller

## Temel Modüller ve Özellikler

### 👨‍💻 Yönetim Paneli

#### Müşteri Yönetim Modülü
- Müşteri ekleme, silme ve düzenleme işlemleri
- Müşteri bilgilerinin detaylı biçimde kaydı
- Filtreleme ve arama fonksiyonları

#### Konaklama Yönetim Modülü
- Ev / oda / apart türü konaklama tiplerinin kaydı
- Her konaklamanın **Durum** bilgisi:
  - 🟢 Müsait: Kiralanabilir durumda
  - 🟠 Kirada: Hâlihazırda kiralanmış
  - 🔴 Çıkarıldı: Artık sistemde olmayan konaklama
- Renk kodlu durum gösterimi
- Konaklama detaylarının düzenlenmesi ve silinmesi

#### Demirbaş Yönetim Modülü
- Satın alınan eşya ve malzemelerin kaydı
- Her demirbaş için **Durum** bilgisi:
  - 🟢 Müsait: Kullanıma hazır
  - 🟠 Kirada: Aktif kullanımda
  - 🔴 Çıkarıldı: Sistemden çıkarılmış / arızalı
- Demirbaş düzenleme, silme ve listeleme

### 🏠 Kiralama Modülü
- Önce müşteri seçimi yapılır
- Sistemde müsait olarak görünen konaklamalar listelenir
- Eşya ihtiyacına göre demirbaşlar seçilebilir (isteğe bağlı)
- Kiralama detayları girilir ve şu ilişkisel bağ kurulur: **Müşteri + Konaklama + (Opsiyonel) Demirbaş**

### 💳 Ödemeler Modülü
- Aylık ödeme takibi
- Otomatik e-posta bildirimleri (hatırlatma ve uyarı)
- Renkli uyarı sistemi:
  - 🔴 Ödemesi Geçen
  - 🟠 Yaklaşan (son 2 hafta)
  - 🟢 Ödemesi Tamamlanan

### 📊 Muhasebe Modülü
- Aylık gelir ve gider girişleri
- Detaylı muhasebe tablosu
- Filtreleme: tarihe, kaleme ve kategoriye göre
- Finansal raporlama altyapısı (ilerleyen sürümlerde PDF/Excel desteği)

## Kullanıcı Rolleri
- **Yönetici:** Tüm modüllere erişim
- **Operasyon Yetkilisi:** Kiralama, konaklama, müşteri yönetimi
- **Muhasebe Yetkilisi:** Ödeme ve gelir-gider modülü
- **Destek Personeli:** Yalnızca görüntüleme yetkisi

