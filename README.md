# Dirty Paws Nedir?

Sokak hayvanlarına yardım etmek isteyen insanların bulundukları konuma göre bir araya geldiği, beraber çalışma yürütebildiği, acil durumlarda (hayvan yaralanması, hastalık, vb.), yakınlarındaki bir insandan yardım isteyebildiği, ettikleri yardımların karşılığında biriktirdikleri puanlar ile anlaşmalı firmalardan çeşitli indirim avantajları elde edebildiği bir mobil uygulamadır. Tasarlanan yapay zeka temelli akıllı mama kapları sayesinde tahmini mama bitiş süresinin, su seviyesinin, kabın içerisine yabancı cisim atılma durumunun, kullanıcılar tarafından anlık olarak izlenebilmesi sağlanmaktadır.

Hackathondan sonraki süreçte
- Reinforcement learning algoritmaları yardımıyla hayvanlar üzerine bağlanan mikro işlemciler ile hareketlerin kaydedilip anomalilerin (kaza, açlık, sağlık sorunları vs.) saptanması ve yakınlardaki kullanıcılara bilgi verilmesi sağlanacak.
- Ödül mekanizması aktif hale getirilecek.
- Uygulama tasarımı aşağıdaki şekilde güncellenecek.

![figmaIMG](https://storage.googleapis.com/dirty-paws.appspot.com/DirtyPawsFigma.png)

Uygulama Akışına [buradan](https://storage.googleapis.com/dirty-paws.appspot.com/dirty-paws-flow-minified%20(1).png) ulaşabilirsiniz 

Projenin kısa tanıtımı için hazırlamış olduğumuz videoya aşağıdaki linkten ulaşabilirsiniz.
[Youtube Link](https://www.youtube.com/watch?v=h_4BVdnsppM&feature=youtu.be)

# Bileşenler ve Kullanılan Teknolojiler

Proje dört ana bileşene sahiptir bunlar. **Backend**, **Mobil Uygulama**, **AI** ve **Akıllı Mama Kaplarıdır**. 

**ÖNEMLİ NOT:** Her bileşinin ilgili klasörlerinde gerekli bilgiler *README.md* dosyalarında özel olarak verilmiştir.<br>

- [Mama Kabı](/Arduino) <br>

```
Arduino Uno Rev 3
LM35 sıcaklık sensörü
ESP8266 WiFi Modül
DHT11 sıcaklık ve nem sensörü
HC-SR04 Ultrasonik sensör
TEM01052B ağırlık sensörü

```

- [AI](/AI) <br>
```
Tensorflow
Resnet50V2
Keras
Scikit-learn
PIL

pip freeze
ipykernel==5.3.4
ipython==7.18.1
ipython-genutils==0.2.0
joblib==0.16.0
jsonpickle==1.4.1
jsonschema==3.2.0
jupyter-client==6.1.7
jupyter-core==4.6.3
jupyterlab-pygments==0.1.1
Markdown==3.2.2
MarkupSafe==1.1.1
notebook==6.1.1
numpy==1.19.2
numpydoc==1.1.0
Pillow==7.2.0
PyMySQL==0.10.1
regex==2020.6.8
scikit-image==0.16.2
scikit-learn==0.22.2.post1
sklearn-crfsuite==0.3.6
spyder==4.1.5
spyder-kernels==1.9.4
SQLAlchemy==1.3.19
sqlparse==0.3.1
statsmodels==0.12.0
tabulate==0.8.7
tensorboard==2.1.1
tensorboard-plugin-wit==1.6.0
tensorflow==2.1.1
tensorflow-addons==0.7.1
tensorflow-estimator==2.1.0
tensorflow-gpu==2.1.0
tensorflow-gpu-estimator==2.1.0
tensorflow-hub==0.8.0
tensorflow-probability==0.9.0
ujson==2.0.3
uritemplate==3.0.1
urllib3==1.25.8
virtualenv==20.0.35
```
- [Backend](/Backend) <br>

```
Django>=3.1.2
djangorestframework
psycopg2-binary>=2.8
tensorflow
sklearn
sklearn-crfsuite==0.3.6
pandas
pickleshare==0.7.5
PyMySQL==0.10.1
keras
requests
Pillow
Google Cloud Platform
```

- [Mobil Uygulama](/Mobile-App) <br>

```
Flutter
environment:
  sdk: ">=2.2.2 <3.0.0"

dependencies:
  flutter:
    sdk: flutter
  flutter_login: 
    path: lib/flutter_login
  font_awesome_flutter: ^8.5.0
  intl: ^0.16.1
  provider: ^4.0.1
  http: ^0.12.2
  cupertino_icons: ^1.0.0
  google_maps_flutter: ^1.0.3
  maps_launcher: ^1.2.2+1
  camera:
  path_provider:
  image_picker:
  path:
  geolocator:
  geocoding:
  permission_handler:
  fluttertoast:
  firebase_core: ^0.4.0+9
  firebase_auth: ^0.14.0+5
  flutter_launcher_icons:
  android_intent:
Figma (UI/UX)

```

# Ekip Üyeleri

**Aysu Demir**

1997 Ankara doğumluyum. Başkent Üniversitesi Bilgisayar ve Endüstri Mühendisliklerinden 2019 yılında mezun oldum. Hali hazırda BOTAŞ’ta yazılım geliştirme departmanında proje yöneticisi ve ODTÜ'de master öğrencisiyim. 3. sınıfta yapay zekaya ilgim başladı ve bitirme projelerimi bu alanda yaptım. Doğal Dil İşleme, Nesne Tanıma, Makine Öğrenmesi algoritmalarıyla projeler yürüttüm. <br>
*Görevler: Makine Öğrenmesi, Derin Öğrenme, Takım Lideri*<br>
İletişim:<br>
*E-mail:* aysuudemiir@gmail.com
  
**Barış Hasdemir**

  Ben Barış, 1995 İstanbul doğumluyum. Doğu Akdeniz Üniversitesi Bilgisayar Mühendisliği 3. Sınıf öğrencisiyim. Microsoft LS Ambassador ve aynı zamanda Google DSC EMU Core Team üyesi olarak faaliyet gösteriyorum. Mobil/Web geliştiricisi olarak çalışma deneyimim oldu. Son bir senedir Makine Öğrenmesi, Derin Öğrenme, Doğal Dil işleme alanlarıyla ilgileniyorum.<br>
*Görevler: Backend, Makine Öğrenmesi, Derin Öğrenme*<br>
İletişim:<br>
E-mail: barishasdemir@gmail.com
  
**Şule Parlat**


İzmir Yüksek Teknoloji Enstitüsü 2. Sınıf Elektronik ve Haberleşme Mühendisliği öğrencisiyim. İzmir Teknopark'ta e-cap isimli projeyi yürütüyorum. Son yıllarda görüntü işlem ve makine öğrenmesi alanlarıyla ilgileniyorum.<br>
*Görevler: Akıllı Mama Kabı, Mobil Uygulama,* <br>
İletişim:<br>
*E-mail:* suleparlat@gmail.com
  
**Barış Dede**
 
Ben Barış, 1996 Ankara doğumluyum. Ankara Üniversitesi Bilgisayar Programcılığı 2017 mezunuyum. Doğu Akdeniz Üniversitesi Bilgisayar Mühendisliği 3. sınıf öğrencisiyim. Uzun yıllardır web tabanlı, son 4 yıldır ise buna ek olarak cross ve native geliştirme ile ilgileniyorum. Google DSC EMU Core Team üyesi olarak faaliyet gösteriyorum.<br>
*Görevler: Mobil Uygulama , UI/UX, Backend*<br>
İletişim:<br>
*E-mail:* baris@barisdede.com<br>


