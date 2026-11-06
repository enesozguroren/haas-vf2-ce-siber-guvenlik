# Haas VF-2 CNC Dik İşleme Merkezi — CE ve Siber Güvenlik İncelemesi

**Ders:** Yazılım Mühendisliği Güncel Konular  
**Hazırlayan:** Enes Özgür Ören  
**Grup:** Gece  
**Tarih:** 23.10.2026  
**Durum:** Kapak + LAB 1–7 tamamlandı (06.11.2026); akademik CE teknik dosyası çalışması ayrıca devam ediyor

## Projenin amacı

Haas VF-2 CNC dik işleme merkezini örnek makine olarak seçerek teknik dokümantasyon, makine emniyeti ve endüstriyel siber güvenlik açısından değerlendirmek; ilerleyen aşamalarda **CE uygunluk değerlendirmesine yardımcı olabilecek akademik bir teknik dosya taslağı** hazırlamak.

Bu repo gerçek bir CE belgesi, resmî sertifikasyon veya makinenin güvenli olduğuna ilişkin test edilmiş bir garanti değildir. Fiziksel makineye erişim ve kontrol yazılımı sürümü doğrulanmadıkça cihazın gerçek durumu hakkında kesin ifadeler kullanılmaz.

## İçerik

| Dosya | Açıklama |
| --- | --- |
| [`docs/Haas_VF2_Laboratuvar_Foyu.pdf`](docs/Haas_VF2_Laboratuvar_Foyu.pdf) | Tamamlanan kapak ve LAB 1–7 bölümleri (8 sayfa). |
| [`analizler/SWOT_Analizi.md`](analizler/SWOT_Analizi.md) | Projenin ve seçilen makinenin güçlü/zayıf yönleri, fırsatlar ve tehditler. |
| [`analizler/SMART_Analizi.md`](analizler/SMART_Analizi.md) | Somut, ölçülebilir, ulaşılabilir, ilgili ve zaman sınırı olan proje hedefleri. |
| [`kaynaklar/Kaynaklar.md`](kaynaklar/Kaynaklar.md) | Üretici ve güvenlik açığı kayıtlarına bağlantılar, kanıt durumu. |
| [`PROJE_KAPSAMI.md`](PROJE_KAPSAMI.md) | Kapsam, varsayımlar ve sonraki teknik dosya adımları. |

## İncelenen makine

- **Üretici / model:** Haas Automation — VF-2
- **Makine türü:** CNC dik işleme merkezi
- **Örnek varlıklar:** CNC kontrol ünitesi, iş mili, hareketli eksenler, operatör paneli, Ethernet bağlantısı, kapı kilidi ve acil durdurma düzeni
- **Bilinmeyenler:** Üretim yılı, seri numarası, kurulu yazılım sürümü, opsiyonlar, gerçek ağ topolojisi ve kurulumun güvenlik doğrulama sonuçları

Üreticinin ürün sayfasında Ethernet arayüzü ve teknik dokümanlar listelenir. Makine özellikleri opsiyonlara göre değişebilir.

## Güvenlik açığı incelemesi

CVE-2022-2474, **Haas CNC Controller 100.20.000.1110** sürümündeki Ethernet Q Commands hizmetine ilişkin bir kayıttır. NVD, CVSS v3.1 temel puanını **8.0 (HIGH)** olarak gösterir; kaynakta farklı kurumların farklı puanlamaları da bulunabilir. **Bu açığın seçilen herhangi bir VF-2'yi doğrudan etkilediği kanıtlanmış değildir.** İlk iş, kontrolcü ve sürüm eşleşmesini doğrulamaktır.

Referans: https://nvd.nist.gov/vuln/detail/CVE-2022-2474

## Çalışma ilkeleri

1. Doğrulanmış ürün verisi, akademik varsayım ve öneriyi açıkça ayır.
2. Fiziksel sistem üzerinde izinsiz tarama, istismar veya kontrol değişikliği yapma.
3. Emniyet fonksiyonları için laboratuvar varsayımını gerçek doğrulama olarak sunma.
4. Gerçek CE uygunluğu beyan etmek yerine örnek teknik dosya taslağı üret.
5. Yeni belge ve test kanıtlarını kaynak/tarih/sürüm bilgisiyle ekle.

## Haftalık güncelleme yöntemi ve tamamlanma durumu

- **06.11.2026 sürümü:** Kapak + LAB 1–7 (8 sayfa). İlk 5 sayfa (kapak ve LAB 1–4) aynen korunmuştur.
- **LAB 5:** SBOM / CVE / Patch değerlendirmesi eklendi.
- **LAB 6:** CRA olay müdahale simülasyonu eklendi.
- **LAB 7:** AI Safety Challenge senaryosu eklendi. Buradaki YZ uygulaması, Haas VF-2 üzerinde doğrulanmış bir donanım özelliği değil, laboratuvar senaryosudur.
- **SWOT ve SMART:** Mevcut analizler saklanmıştır. Sonraki teknik dosya aşamalarında gerekirse ayrıca revize edilebilir.
- **Revizyon disiplini:** Yeni teknik dosya kanıtları ve değişiklikler, ayrı Git commit'leriyle izlenir.

| Bölüm | Repo durumu |
| --- | --- |
| Kapak ve LAB 1–4 | Tamamlandı / PDF’de |
| LAB 5 | Tamamlandı / PDF’de |
| LAB 6 | Tamamlandı / PDF’de |
| LAB 7 | Tamamlandı / PDF’de |
| CE teknik dosyası | Hazırlık / ayrıca geliştirilecek |

## Planlanan devam

Teknik doküman ve sürüm envanteri → makine emniyeti kapsamı → varlık/ağ mimarisi → risk analizi → CVE uygunluk kontrolü → güvenlik gereksinimleri → kanıt matrisi → akademik CE teknik dosya taslağı.
