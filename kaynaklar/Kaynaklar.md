# Kaynaklar ve Doğrulama Durumu

**Erişim / derleme tarihi:** 23.10.2026

| Kaynak | Kapsam | Durum |
|---|---|---|
| [Haas VF-2 ürün sayfası (TR)](https://www.haascnc.com/tr/machines/vertical-mills/vf-series/models/small/vf-2.html) | Model özellikleri, Ethernet, teknik belgeler | Üretici kaynağı |
| [Haas VF-2 ürün sayfası (EN)](https://www.haascnc.com/machines/vertical-mills/vf-series/models/small/vf-2.html) | Kılavuz ve kurulum bağlantıları | Üretici kaynağı |
| [Haas frezeleme için uygunluk bilgileri](https://www.haascnc.com/service/service-content/guide-procedures/legal-information---mill-doc.html) | Üretici uygunluk beyanı / hukuki bilgi | Belirli konfigürasyon için uygulanabilirliği kontrol edilmeli |
| [NVD CVE-2022-2474](https://nvd.nist.gov/vuln/detail/CVE-2022-2474) | Haas kontrolcü 100.20.000.1110, Ethernet Q Commands | Gerçek CVE; VF-2 kurulumuna uygulanması doğrulanmadı |
| [CISA ICSA-22-298-01](https://www.cisa.gov/news-events/ics-advisories/icsa-22-298-01) | Haas kontrolcü siber güvenlik duyurusu | Referans olarak kullanılabilir |

## CVE değerlendirme kaydı

- **CVE:** CVE-2022-2474
- **Etkilenen ürün/sürüm:** Haas CNC Controller 100.20.000.1110
- **Açıklama:** Ethernet Q Commands hizmetinin kimlik doğrulama eksikliği nedeniyle yetkisiz makro yazılabilmesi
- **NVD CVSS v3.1:** 8.0 (High); NVD sayfasında CNA değerlendirmesi farklı olabilir
- **Makinemize uygulanabilirlik:** **Bilinmiyor** — gerçek kontrolcü sürümü doğrulanmalı
- **Gerekli kanıt:** CNC kontrolcü yazılım sürümü, Ethernet Q Commands hizmetinin yapılandırması, ağ erişilebilirliği ve üretici güncelleme durumu

Burada verilen bilgiler, mevcut VF-2 kurulumunda güvenlik açığı bulunduğu iddiası değildir.
