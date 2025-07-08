# Alzheimer Tespiti için Hipokampus Tabanlı Derin Öğrenme Projesi

Bu proje, TÜBİTAK 2209-A desteği kapsamında geliştirilmiştir. Amaç, Alzheimer hastalığının erken teşhisi için hızlı, güvenilir ve yüksek doğruluk oranına sahip bir derin öğrenme modeli geliştirmektir.

Araştırmada, Alzheimer Hastalığı Nöro Görüntüleme Girişimi (ADNI) veri tabanından temin edilen MRI görüntüleri kullanılmıştır. Öncelikle, `.nii` uzantılı MRI dosyalarına `registration.ipynb` dosyası ile görüntü hizalama (registration) işlemi uygulanmıştır.

Daha sonra, `slicekaydetme.ipynb` dosyasıyla hipokampus bölgesinin en belirgin olduğu 5 dilim (slice) seçilmiştir. Bu görüntüler, `labelImg` programı kullanılarak etiketlenmiştir.

Son aşamada, elde edilen veriler üzerinde **YOLOv5**, **YOLOv7** ve **YOLOv9** modelleri eğitilerek Alzheimer tespiti gerçekleştirilmiştir.
