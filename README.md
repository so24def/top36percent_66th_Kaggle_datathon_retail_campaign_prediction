# Datathon - Harcanan Tutara Göre Müşterilerin Kampanyaya Katılma Tahmini

  
### Bu yarışmayı Kaggle üzerinden düzenleyen şirket, datathon bittikten bir süre sonra verilerinin gizlilğini sağlamak kapsamında benimle iletişime geçerek paylaştığım yarışma çözümümü gizliye almamı rica etti. Şirket tarafından paylaşılan ham veriler görünmeyecek şekilde çözümümü paylaşmanın herhangi bir sorun yaratmayacağını teyit ettikten sonra, sadece yarışma esnasında izlediğim yolları ve çözümleri paylaşabilmek adına çalışmamı ham veriler olmadan ve gözükmeden tekrar yüklemiş bulunmaktayım.

  Ham verilerle henüz bir tecrübem olmamasına rağmen, sadece kendimi test etmek adına ve herhangi bir beklentim olmadan katıldığım, ancak sadece son dört gününde katılım sağlayabildiğim bu yarışmada katılımcılardan beklenen;
  
  Şirket tarafından paylaşılan kullanıcı verileri ile, kullanıcının kendisine belirtilen X kadar miktar daha alışveriş yapar ise Y kadar bir ödül puanı kazanacak olması kampanyasına katılım sağlaması(1) veya sağlamaması(0) durumlarının tahminini sağlamak ve en yüksek F1 skoruna sahip modeli oluşturmaktı.
  
  Ham veriyi incelerken ve düzenlerken, daha sonrasında da feature engineering yaparak birleştirirken farkettiğim üzere hedef dağılımı(response) yaklaşık %98 oranında 0 ve %2 oranında 1 içermekteydi ve çok dengesiz idi. 
  
  Bu veri seti üzerinde denemek üzere çok sayıda model ile cross-validation ve mutual info yöntemiyle feature selection yaptım, GridCV/RandomizedSearchCV yöntemleri ile veri setine en uygun modeller için optimal hiperparametreleri seçmeye çabaladım. Daha sonrasında veri setindeki dengesizlikle ilgilenmek üzere, modellerde overfittinge yol açmamaya dikkat edecek şekilde, hedef değişkeninde azınlık olan noktaları artırmak ve modelin ezbere bir şekilde çoğunluk olan response değerini tahmin etmesi ihtimalini azaltmayı hedefleyerek oversampling uyguladım. 
  
  Sonuç olarak bu yarışmayı; toplamda 287 katılımcı ve 186 takım içerisinden bireysel olarak 66. sırada(top %36) tamamlamak kendim için beklediğimden iyi bir sonuçtu. Son dört günde katılma fırsatım olduğu için ve günlük olarak yapılabilen submission sayısı sınırlı olduğu için, oluşturduğum modelleri daha da iyileştirme ve genelleştirme, böylelikle daha yüksek F1 skorları elde edebilme fırsatını kaçırmış oldum.
  
  Eklemiş olduğum notebook dosyalarında yarışma boyunca yaptığım çalışmaların temize çekilmiş hali ve daha fazla detay bulunmaktadır. Tecrübe sahibi olmadığım konuları yarışma esnasında araştırıp, öğrenip, uygulamış olmam sebebiyle çalışma dosyalarım çok karmaşık ve okunamaz bir hale gelmişti, o sebeple temize çekip buraya eklemeyi tercih ettim.



https://www.kaggle.com/so24def
