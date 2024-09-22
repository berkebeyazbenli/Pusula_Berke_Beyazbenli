# Pusula_Berke_Beyazbenli
--Data Science Intern Case Study--

Bu proje, ilaç kullanımına bağlı olarak bildirilen yan etkilerin analizine odaklanmaktadır. Veriler; kullanıcı bilgilerini, ilaç başlangıç ve bitiş tarihlerini, ilaç isimlerini, yan etkileri ve çeşitli özellikleri içermektedir. Analiz süreci, verilerin temizlenmesi, eksik verilerin doldurulması ve görselleştirilmesi üzerine yoğunlaşmıştır.

<br>
Veri Seti Hakkında
Veri seti toplamda 2357 satır ve 19 sütun içermektedir. İçerdiği bilgiler:

Kullanıcı kimliği: Kullanici_id <br>
Cinsiyet: Cinsiyet <br>
Doğum tarihi: Dogum_Tarihi <br>
Uyruk: Uyruk <br>
İl: Il <br>
İlaç adı: Ilac_Adi <br>
İlaç başlangıç ve bitiş tarihleri: Ilac_Baslangic_Tarihi, Ilac_Bitis_Tarihi <br>
Yan etki bilgisi: Yan_Etki <br>
Yan etki bildirim tarihi: Yan_Etki_Bildirim_Tarihi <br>
Alerjiler ve kronik hastalıklar <br>
<br>
Eksik Veriler
Veri setinde bazı sütunlarda eksik veriler mevcuttur:

Cinsiyet: 778 eksik <br>
İl: 227 eksik <br>
Alerjilerim: 484 eksik <br>
Kronik Hastalıklarım: 392 eksik <br>
Verilerin eksik olduğu durumlarda iki yöntem kullanılmıştır:

Sayısal veriler için eksik değerler, ortalama ile doldurulmuştur (Kilo, Boy).
Kategorik veriler için ise en çok tekrar eden veri ile doldurulmuştur.
<br>
Veri Dönüşümü
Label Encoding ve One-Hot Encoding: Kategorik değişkenler LabelEncoder ile kodlanmış, sıralı olmayan değişkenler get_dummies yöntemiyle sayısallaştırılmıştır.

Yaş Hesaplama: Kullanıcıların doğum tarihine göre yaşı hesaplanmış ve veri setine yeni bir sütun olarak eklenmiştir. Bu işlem sonrası Dogum_Tarihi sütunu çıkarılmıştır.

Ölçeklendirme: Boy, kilo, yaş gibi değişkenler arasındaki büyük farkları gidermek için MinMaxScaler kullanılarak veriler normalize edilmiştir. Böylece makine öğrenimi modelleri için veriler uygun hale getirilmiştir.

<br>
Sonuçlar
Veri seti üzerinde yapılan ön analizler, veri temizleme ve dönüştürme işlemleri sonrasında kullanıma hazır hale getirilmiştir. Eksik verilerin tamamlanması ve ölçeklendirilmesi ile daha anlamlı sonuçlar elde edilmiştir. Bu analiz, ilaçlara bağlı yan etkilerin daha derinlemesine incelenmesine olanak sağlamaktadır.

Gelecek adımlarda bu veri seti, istatistiksel modelleme ve makine öğrenimi algoritmaları için kullanılabilir hale getirilmiştir.

<br>

