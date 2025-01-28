# Brain Tumor Dataset Analysis and Processing

This project involves processing and analyzing medical images using Python.

## Table of Contents

- 2- İndirdiğim .json dosyasını çağırdım.
- 3- Kaggle'da üzerinde çalıştığım veri setinin ilk yükleyicisinin sahibi bulup profilinden veri setini çektim.
- 4- Veri setini unzip yaptım. İçeriğini indirdim.
- 5- Veri setinin içeriğini görüntüledim.
- Brain - Tumor Datasetini ve içinde bulunan klasörleri listeledim.
- (Dosya yoluna bakmam gerekti)
- Dataset içinde her alt klasördeki görüntüleri listeledim ve işlemek üzere organize ettim.
- Görüntü İşleme Fonksiyonları
- Görüntüleri İşleme ve Kaydetme
- İşlenmiş Görüntüleri Görüntüleme
- Her kategori için orjinal ve işlenmiş görüntülerin gösterilmesi
- Orjinal görüntü üzerinde Erozyon, Openning Closing ve Gradyan işlemlerinin yapıldığı kısım (hepsinin üst üste yapıldığı durum)
- Orjinal görüntü üzerinde Erozyon, Openning Closing ve Gradyan işlemlerinin yapıldığı kısım (ayrı ayrı yapıldığı kısım)
- Kontrast, keskinlik, parlaklık, renk doygunluğu ayarı yapıldıktan sonra aynı görüntü üzerinde önce erozyon sonra sırasıyla yine aynı görüntü üzerinde açılma, kapanma ve gradient uygulandı.
- Kontrast,keskinlik, parlaklık, renk doygunluğu yapıldıktan sonra işlenmiş görüntü üzerinde tek tek ve ayrı ayrı erosyon, açılma, kapanma, gradient ayarı yapıldı
- Pre_Process edilmiş tüm görüntüler üzerinde "Erozyon, Opening, Closing ve Gradient" işlemleri uygulanıp ardından bu işlemlerin sonuçları işlem isimleri ile birlikte yeni bir "post_processed_images" klasörüne kaydediliyor.
- Bütün dosyalarıma bakıyorum kayıt olmuşlar mı diye
- Bir görüntü çağrılarak "hem orjinal hali hemde  işlenmiş olan haline" R-G-B uygulanmıştır
- ROI Sobel ve Canny Kenar tespiti yapılan kısım
- Orjinal görüntüler için ROI ve ardından sobel ve canny uygulandı ve her biri farklı dosya yapıları olarak kaydedildi
- Pre_processed görüntüler için ROI ve ardından sobel ve canny uygulandı ve her biri farklı dosya yapıları olarak kaydedildi
- SEGMENTASYON
- 1 eşikleme yöntemleriyle bir görüntüyü binarize eder
- 2 filtreler uygulanarak görüntüde değişiklikler yapılır
- 3 Kontur uygulanması
- 4 GrabCut Segmentasyonu
- 9 Otsu yöntemiyle eşikleme yaparak görüntüyü binary (ikili) hale getirir. Son olarak, orijinal ve eşiklenmiş görüntüleri ekranda gösterir.
- 10 Etiketleme ve Watershed Algoritması:
- 11  flood fill

## How to Use

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```
2. Navigate to the project directory:
    ```bash
    cd your-repo-name
    ```
3. Open the Jupyter notebook:
    ```bash
    jupyter notebook Medical_Image_Processing.ipynb
    ```

## Requirements

- Python 3.x
- Jupyter Notebook
- Required libraries: (add library names here, e.g., NumPy, Matplotlib, etc.)

## Project Structure

- `Medical_Image_Processing.ipynb`: Main notebook for medical image processing.
- `data/`: Directory to store input medical images (create this folder if it doesn't exist).
- `results/`: Directory to store output processed images and analysis results.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes or suggestions.

---

Generated from the `Medical_Image_Processing.ipynb` file.
