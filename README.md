Frichats (Sohbet uygulaması)


Basit bir tasarıma sahip bir giriş formu gibi görünüyor. İçinde bir başlık ve bir form bulunan 
bir kap elemanına sahiptir. Formda, kullanıcının e-posta adresini ve parolasını girmesi için iki 
giriş alanı ve oturum açmak için bir gönder düğmesi bulunur. Ayrıca yeni bir hesap oluşturmak 
için bir bağlantı ve ana sayfaya geri dönmek için bir düğme vardır. HTML dosyası ayrıca CSS 
(Basamaklı Stil Sayfaları) kullanan bazı satır içi stiller de içerir. 


asd.html  Kısmı
Biri kullanıcının kullanıcı adı, diğeri de mesaj göndermek istediği kişinin kullanıcı adı için 
olmak üzere iki giriş alanı içeren bir form ve bir gönder düğmesi içeren bir HTML dosyasıdır. 
Form gönderildiğinde, message.html sayfasına sorgu dizesindeki giriş alanlarının değerlerini 
içeren bir GET isteği gönderir. 


index.js  Kısmı
Express.js sunucusu ve .js sunucusu ayarlayan düğüm Socket.io bir dosyadır. Express.js sunucusu, 
80 numaralı bağlantı noktasındaki (veya ayarlanmışsa işlemin ortam değişkeni PORT) istekleri 
dinler. Belirli istekleri aldığında, belirtilen dosyayı geri gönderir. Socket.io sunucusu 801 
numaralı bağlantı noktasını dinler ve bağlantılar ve bağlantı kesilmeleri için olay 
dinleyicileri ayarlar. Belirli bir md5 değerine sahip bir mesaj aldığında, mesajı bağlı tüm 
istemcilere yayınlar. 


message.html Kısmı
MD5 karma işlevinin bir uygulamasını içeren bir JavaScript dosyasıdır. MD5 karma işlevi bir 
giriş ("d" olarak adlandırılır) alır.


styles.css  Kısmı
Sohbet mesajlarının, giriş alanının ve gönder düğmesinin düzenini ve görünümünü tanımlar. Ayrıca 
yazı tipini Helvetica veya Arial olarak ayarlar ve tüm öğelerin kenarlık kutusunun kutu boyutuna 
sahip olması gerektiğini belirtir. Sohbet mesajları, sırasıyla kullanıcı tarafından gönderilen 
ve diğer kullanıcılardan alınan mesajların arka planını ve metin renklerini belirten "mesaj 
gönderen" ve "mesaj alıcı" olmak üzere iki sınıfa ayrılır. İletilere ayrıca cilalı bir görünüm 
kazandırmak için bir doldurma, kenar boşluğu, kenarlık yarıçapı ve genişlik verilir. Giriş 
alanına ve gönder düğmesine sayfanın altında sabit bir konum verilir ve arka plan rengi ve metin 
rengiyle stillendirilir. 
