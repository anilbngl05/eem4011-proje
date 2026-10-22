# eem4011-proje
Proje 2: Telefon Kamerasıyla Nabız Tespiti (BUT PPG)
Bu projede akıllı telefon kamerasıyla parmaktan kaydedilmiş 10 saniyelik PPG (fotopletismogram) sinyalleri üzerinden tepe noktaları sayılarak nabız (HR) hesaplanmakta ve eş zamanlı EKG referans nabız değerleri ile karşılaştırılmaktadır.

Veri Seti
Veri Seti Adı: BUT PPG Database v2.0.0

İndirme / Erişim Linki: https://physionet.org/content/butppg/2.0.0/

Not: Veri seti boyutu ve kurallar gereği ham veri dosyaları depoya eklenmemiştir. Kod, PhysioNet üzerinden gerekli kayıtları (quality-hr-ann.csv, subject-info.csv ve koşulu sağlayan ilk 100 kaydı) doğrudan çekerek çalıştırmaktadır.

Çalıştırma Adımları
Depodaki .ipynb uzantılı notebook dosyasını Google Colab üzerinde açın.

Gerekli bağımlılıkların (wfdb, numpy, scipy, matplotlib, pandas) kurulu olduğundan emin olun (gerekiyorsa ilk hücrede !pip install wfdb çalıştırın).

Hücreleri sırasıyla baştan sona çalıştırın.

Kod çalıştığında ilk kayda ait görsel (sekil1.png) üretilecek ve 100 kaydın klasik tepe sayma metrikleri baseline.csv dosyasına kaydedilecektir.

Ana Sonuçlar
100 adet PPG kaydı (Ear/finger = 1, Quality = 1) üzerinde yapılan ham tepe sayma yöntemi analizi sonucunda elde edilen baseline performans:

İşlenen Kayıt Sayısı: 100

Baseline MAE: ___ atım/dk

Hata < 5 atım/dk Yüzdesi: %___
