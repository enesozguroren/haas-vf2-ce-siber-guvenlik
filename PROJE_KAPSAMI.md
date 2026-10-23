# Proje Kapsamı ve CE Teknik Dosyası Hazırlık Notları

## Seçilen nesne

**Haas Automation VF-2 CNC dik işleme merkezi.** İncelenen şey belli bir tesisteki seri numaralı fiziksel makine değil, kamuya açık üretici belgeleri üzerinden ele alınan modeldir.

## Verilerin sınıflandırılması

- **Doğrulandı:** Üreticinin VF-2 modelini ve Ethernet arayüzünü belgelediği; CVE-2022-2474'ün belirli Haas kontrolcü sürümünü etkilediği.
- **Henüz bilinmiyor:** Örnek makinenin üretim yılı, opsiyonları, denetleyici sürümü, ağ yapılandırması ve gerçek risk azaltma doğrulaması.
- **Akademik tasarım önerisi:** Ağ bölgelendirme, erişim kuralları, kayıt tutma ve belgelendirme planı. Bunlar makinede fiilen kurulu olarak iddia edilmez.

## Hazırlanacak akademik teknik dosya bölümleri (taslak)

1. Makine tanımı, model ve kapsam
2. Üretici dokümanları ve teknik özellikler
3. İlgili mevzuat ve uygulanabilir standartların gerekçeli listesi
4. Makine emniyeti tehlikeleri ve risk değerlendirmesi
5. CNC kontrolcü, yazılım/firmware, ağ bağlantıları ve varlık envanteri
6. Bilinen zafiyetler için model/sürüm/erişim koşulu analizi
7. Siber güvenlik riskleri ve risk azaltma önerileri
8. Emniyet ile siber güvenlik arasındaki bağımlılıklar
9. Test/doğrulama planı ve yapılmayan testlerin listesi
10. Kaynaklar, kanıt matrisi, revizyon geçmişi

## Kritik sınır

Resmî uygunluk dosyası üreticinin/yetkili tarafın teknik ölçümlerini, çizimlerini, risk değerlendirmesini ve mevzuat gereği gerekli diğer kanıtlarını gerektirir. Bu GitHub reposu bunların yerine geçmez.

## Föy ile ilişkinin sınırı

`docs/` içindeki PDF, **yalnızca kapak + LAB 1–4 (toplam 5 sayfa)** içerir. LAB 5, LAB 6 ve LAB 7 henüz eklenmemiştir; ders ilerledikçe tamamlanan sayfalar aynı PDF’ye sırasıyla eklenecektir. Haftalık föy ile dönemin CE teknik dosyası **aynı teslim değildir**; repo teknik dosya çalışmalarıyla ayrıca genişletilebilir.
