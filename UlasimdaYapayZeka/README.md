UlasimdaYapayZeka
TEKNOFEST 2025 Havacılıkta Yapay Zeka Yarışması için geliştirilen bir projedir. Bu proje, hava aracı görüntülerinden nesne tespiti (taşıt, insan, UAP, UAI) ve konum tahmini görevlerini gerçekleştirir.
Kurulum

Depoyu Klonlayın:
git clone https://github.com/kullanici-adi/UlasimdaYapayZeka.git
cd UlasimdaYapayZeka


Geliştirme Ortamını Kurun:

Visual Studio Code ve Dev Containers eklentisini yükleyin.
.devcontainer klasöründeki yapılandırma ile ortam otomatik olarak kurulur.
Alternatif olarak, bağımlılıkları manuel yükleyin:pip install -r requirements.txt




Veri Seti Oluşturma:

Videolarınızı create_dataset.py ile işleyin:python create_dataset.py





Kullanım

Veri Seti Oluşturma: create_dataset.py ile videolardan kareler ayıklayın ve etiketleme yapın.
Model Eğitimi: YOLOv8 ile nesne tespiti modelini eğitin:yolo train model=yolov8n.pt data=dataset/data.yaml epochs=50 imgsz=640



Katkıda Bulunma

Depoyu fork edin.
Yeni bir branch oluşturun: git checkout -b feature/yeni-ozellik.
Değişikliklerinizi commit edin: git commit -m 'Yeni özellik eklendi'.
Push edin: git push origin feature/yeni-ozellik.
Pull request oluşturun.

Lisans
Bu proje MIT Lisansı ile lisanslanmıştır. Detaylar için LICENSE dosyasına bakın.
