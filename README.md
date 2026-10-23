# Haas VF-2 CNC Dik İşleme Merkezi — CE ve Siber Güvenlik İncelemesi

**Ders:** Yazılım Mühendisliği Güncel Konular  
**Hazırlayan:** Enes Özgür Ören  
**Grup:** Gece  
**Tarih:** 23.10.2026  
**Durum:** Kapak + LAB 1–4 tamamlandı (23.10.2026); sonraki laboratuvarlar haftalık eklenecek

## Projenin amacı

Haas VF-2 CNC dik işleme merkezini örnek makine olarak seçerek teknik dokümantasyon, makine emniyeti ve endüstriyel siber güvenlik açısından değerlendirmek; ilerleyen aşamalarda **CE uygunluk değerlendirmesine yardımcı olabilecek akademik bir teknik dosya taslağı** hazırlamak.

Bu repo gerçek bir CE belgesi, resmî sertifikasyon veya makinenin güvenli olduğuna ilişkin test edilmiş bir garanti değildir. Fiziksel makineye erişim ve kontrol yazılımı sürümü doğrulanmadıkça cihazın gerçek durumu hakkında kesin ifadeler kullanılmaz.

## İçerik

| Dosya | Açıklama |
| --- | --- |
| [`docs/Haas_VF2_Laboratuvar_Foyu.pdf`](docs/Haas_VF2_Laboratuvar_Foyu.pdf) | Şu ana kadar tamamlanan kapak ve LAB 1–4 bölümleri (5 sayfa). Bu aşamada LAB 5–7 repoda yer almaz. |
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

## Haftalık güncelleme yöntemi

- **Mevcut sürüm:** Kapak + LAB 1, LAB 2, LAB 3 ve LAB 4 (5 sayfa).
- **LAB 5 işlendiğinde:** Önceki sayfaları koruyarak tamamlanan LAB 5 sayfası PDF’ye eklenir; değişiklik yeni bir Git commit’i olarak yayımlanır.
- **LAB 6 ve LAB 7:** Aynı şekilde yalnızca tamamlandıktan sonra eklenir.
- **SWOT ve SMART:** Analizler proje kapsamı ve yeni bulgular geliştikçe revize edilir; kayıtlarda doğrulanmış bilgi ile varsayımlar ayrılır.
- **Revizyon disiplini:** Her haftaki commit mesajında eklenen laboratuvar, tarih ve temel değişiklik yazılır.

| Bölüm | Repo durumu |
| --- | --- |
| Kapak ve LAB 1–4 | Tamamlandı / PDF’de |
| LAB 5 | Henüz eklenmedi |
| LAB 6 | Henüz eklenmedi |
| LAB 7 | Henüz eklenmedi |

## Planlanan devam

Teknik doküman ve sürüm envanteri → makine emniyeti kapsamı → varlık/ağ mimarisi → risk analizi → CVE uygunluk kontrolü → güvenlik gereksinimleri → kanıt matrisi → akademik CE teknik dosya taslağı.
