# Pusula_Berke_Beyazbenli
--Data Science Intern Case Study--

--Run Code

#Anaconda app üzerinde jupyter.notebook kullanıldı


---Bu proje, ilaç kullanımına bağlı olarak bildirilen yan etkilerin analizine odaklanmaktadır. Veriler, kullanıcı bilgilerini, ilaç başlangıç ve bitiş tarihlerini, ilaç isimlerini, yan etkileri ve çeşitli özellikleri içermektedir. Analiz süreci, verilerin temizlenmesi, eksik verilerin doldurulması ve görselleştirilmesi üzerine yoğunlaşmıştır.

--Veri setinin genel yapısını anlamak için histogramlar çizilmiştir. Histogramlar ilaç başlangıç ve bitiş tarihleri, kilo, boy gibi sayısal değişkenlerin dağılımını göstermektedir.

##Veri Seti.

#--Veri seti, toplamda 2357 satır ve 19 sütundan oluşmaktadır. İçerdiği bilgiler arasında şunlar bulunmaktadır:

#-Kullanıcı kimliği (Kullanici_id)

#-Cinsiyet (Cinsiyet)

#-Doğum tarihi (Dogum_Tarihi)

#-Uyruk (Uyruk)

#-İl (Il)

#-İlaç adı (Ilac_Adi)

#-İlaç başlangıç ve bitiş tarihleri (Ilac_Baslangic_Tarihi, Ilac_Bitis_Tarihi)

#-Yan etki bilgisi (Yan_Etki)

#-Yan etki bildirim tarihi (Yan_Etki_Bildirim_Tarihi)

#-Alerjiler ve kronik hastalıklar

##Eksik Veriler

#--Veri setinde bazı sütunlarda eksik veriler mevcuttur. Aşağıdaki sütunlar eksik değerlere sahiptir:

#-Cinsiyet: 778 eksik

#-Il: 227 eksik

#-Alerjilerim: 484 eksik

#-Kronik Hastaliklarim: 392 eksik

#** Bazı ihtiyaçlarımıza göre mesela il sütunundaki verileri "dropna" ile düşürülebilir. Bunun üzerinede denemeler yaptım.

##Eksik verilerin yönetimi için iki yöntem kullanılmıştır:

#--Sayısal veriler için eksik değerler, ortalama ile doldurulmuştur (Kilo, Boy) gibi.

#--Kategorik değişkenler LabelEncoder ile kodlanmış, sıralı olmayan değişkenler get_dummies yöntemi ile sayısal verilere dönüştürülmüştür.

##Yaş Hesaplama

#--Doğum tarihine dayalı olarak her kullanıcının yaşı hesaplanmış ve veri setine yeni bir sütun olarak eklenmiştir. Dogum_Tarihi sütunu bu işlem sonrasında veri setinden çıkarılmıştır.

##Verilerin Ölçeklendirilmesi

#--Kan grubu, kilo, boy ve yaş verileri arasında büyük farklılıkları gidermek için MinMaxScaler kullanılmış ve veriler normalize edilmiştir. Bu sayede modelleme ve analiz işlemleri için veriler uygun bir formata getirilmiştir.

##Sonuçlar

#--Veri seti üzerinde yapılan ön analizler, temizleme ve dönüştürme işlemleri sonucunda kullanıma hazır hale getirilmiştir. Eksik verilerin tamamlanması ve ölçeklendirilmesi ile daha anlamlı sonuçlar elde edilmesi için veri hazırlanmıştır. 

#--Bu analiz, ilaçlara bağlı yan etkilerin daha derinlemesine incelenmesine olanak sağlamaktadır. İlerideki adımlar, bu veriler üzerine istatistiksel modelleme, makine öğrenimi algoritmaları için veri-seti düzenlendi


