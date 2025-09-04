# Pusula_Data Science Intern Case (2025)
**Hazırlayan:** Buse Melike Dalbaş
**E-posta:** bmelikedalbas@gmail.com
## Proje Amacı:
Bu çalışmada fizik tedavi ve rehabilitasyon alanına ait 2235 gözlem ve 13 özellikten oluşan bir veri seti incelenmiştir. Hedef değişken TedaviSuresi olup, veri temizlenerek modellemeye hazır hale getirilmiştir. Amaç, veri setindeki eksik ve tutarsız değerleri gidermek, uygun veri dönüşümleri yapmak ve veri setini tahminleme yapmaya hazır hale getirmektir.
## Veri Seti Özellikler:
HastaNo          Hasta ID
Yas              Nümerik
Cinsiyet         Kategorik
KanGrubu         Kategorik
Uyruk            Kategorik
KronikHastalik   String
Bolum            Kategorik
Alerji           String
Tanilar          String
TedaviAdi        Kategorik
TedaviSuresi     Hedef Değişken
UygulamaYerleri  String
UygulamaSuresi   Kategorik
## Yapılan Çalışmalar:
## EDA
Veri seti boyutu incelendi, eksik değerler incelendi, histogram, barchart, korelasyon matrisi gibi görseller oluşturuldu.
## Veri Önişleme:
TedaviSuresi, UygulamaSuresi sayısal ifadeye dönüştürüldü, eksik değerler dolduruldu.
Cinsiyet, Uyruk KanGrubu kolonalarına LabelEncoding, Tanılar, TedaviAdı kolonalrına one-hot encoding işlemleri uygulandı.
Metin bazlı kolonlar üzerinde KronikHastalık gibi TF-IDF vektörleşme uygulandı.
Yas, TedaviSuresi, UygulamaSuresi kolonlardında StandartScaler uygulandı.
## Sonuç:
Veri seti temizlenmiş, eksik değerlerden arındırılmış ve kategorik değişkenler encode edilmiştir.
Hedef değişken TedaviSuresi modelleme için hazır hale getirilmiştir.
Çalışma sonunda bazı modellemeler karşılaştırılarak tahminleme yapılmış ve sonucunda Rastgele Orman en iyi model bulunmuştur.
## Kullanılan Kütüphaneler:
pandas, numpy, matplotlib, seaborn, scikit-learn
