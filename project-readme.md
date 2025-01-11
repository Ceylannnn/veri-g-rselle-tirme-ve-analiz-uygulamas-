# Veri Görselleştirme Uygulaması

Bu uygulama, CSV dosyalarından veri okuyup çeşitli grafik tipleriyle görselleştirmenizi sağlayan kullanıcı dostu bir Python aracıdır. Uygulama, veri analizi ve görselleştirme işlemlerini kolaylaştırmak için tasarlanmıştır.

## Özellikler

- CSV dosyası okuma ve işleme
- Çeşitli grafik tipleri desteği:
  - Histogram
  - Dağılım Grafiği
  - 3D Dağılım Grafiği
  - Çubuk Grafiği
  - Pasta Grafiği
  - Alan Grafiği
- Türkçe karakter desteği
- Sütun bazlı veri seçimi
- Özelleştirilebilir grafik parametreleri
- Kullanıcı dostu arayüz

## Gereksinimler

```
Python 3.x
pandas
matplotlib
seaborn
plotly.express
tkinter
```

## Kurulum

1. Gerekli Python kütüphanelerini yükleyin:
```bash
pip install pandas matplotlib seaborn plotly
```

2. Projeyi klonlayın veya indirin:
```bash
git clone [proje-url]
cd veri-gorsellestirme
```

3. Uygulamayı çalıştırın:
```bash
python main.py
```

## Kullanım

1. Uygulamayı başlatın
2. "Dosya Seç" butonuna tıklayarak bir CSV dosyası seçin
3. Grafik tipini dropdown menüden seçin
4. Gerekli sütunları seçin:
   - X Sütunu
   - Y Sütunu (gerektiğinde)
   - Z Sütunu (3D grafikler için)
   - Renk Sütunu (opsiyonel)
   - Boyut Sütunu (opsiyonel)
5. "Görselleştir" butonuna tıklayarak grafiği oluşturun

## Grafik Tipleri ve Kullanım Alanları

### Histogram
- Tek değişkenli veri dağılımlarını göstermek için kullanılır
- Sadece X sütunu seçimi gereklidir
- Opsiyonel renk sütunu ile gruplandırma yapılabilir

### Dağılım Grafiği
- İki değişken arasındaki ilişkiyi gösterir
- X ve Y sütunu seçimi gereklidir
- Renk ve boyut sütunları ile ek boyutlar eklenebilir

### 3D Dağılım Grafiği
- Üç değişken arasındaki ilişkiyi gösterir
- X, Y ve Z sütunu seçimi gereklidir
- Renk ve boyut sütunları ile ek boyutlar eklenebilir

### Çubuk Grafiği
- Kategorik verilerin karşılaştırılması için kullanılır
- X ve Y sütunu seçimi gereklidir
- Renk sütunu ile gruplandırma yapılabilir

### Pasta Grafiği
- Bütünün parçalara bölünmesini gösterir
- X (etiketler) ve Y (değerler) sütunu seçimi gereklidir

### Alan Grafiği
- Zaman serisi veya sürekli verileri göstermek için kullanılır
- X ve Y sütunu seçimi gereklidir

## Hata Çözümleri

1. Türkçe Karakter Sorunu
   - Uygulama varsayılan olarak 'DejaVu Sans' font ailesi kullanır
   - Font ailesini değiştirmek için `plt.rcParams['font.family']` parametresini güncelleyin

2. CSV Dosyası Okuma Hatası
   - CSV dosyanızın UTF-8 formatında olduğundan emin olun
   - Dosya yolunda Türkçe karakter olmadığından emin olun

3. Grafik Görüntüleme Sorunları
   - Gerekli sütunların seçili olduğundan emin olun
   - Veri tiplerinin uyumlu olduğunu kontrol edin

## Katkıda Bulunma

1. Projeyi fork edin
2. Feature branch oluşturun (`git checkout -b feature/yeniOzellik`)
3. Değişikliklerinizi commit edin (`git commit -am 'Yeni özellik eklendi'`)
4. Branch'inizi push edin (`git push origin feature/yeniOzellik`)
5. Pull Request oluşturun

## Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için `LICENSE` dosyasına bakın.

## İletişim

CEYLAN ULUSOY
ulusoyceylan09@gmail.com


---
**Not:** Bu uygulama eğitim ve araştırma amaçlı geliştirilmiştir. Profesyonel kullanım için test edilmesi önerilir.
