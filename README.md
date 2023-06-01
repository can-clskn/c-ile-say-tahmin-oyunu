# c-ile-say-tahmin-oyunu
c# ile sayı tahmin etmemize yarayan oyun.
Bu kod, basit bir sayı tahmin oyununu içerir. Form1 sınıfı, Windows Forms uygulamasındaki bir formu temsil eder. Kod, kullanıcının bir sayı girmesine izin verir ve bu sayıyı rastgele belirlenen bir hedef sayıyla karşılaştırır.

Oyunun işleyişi şu şekildedir:

İlk başta, rastgele bir sayı üretilir ve bul değişkenine atanır.
Kullanıcı sayıyı girdiği zaman textBox1_KeyPress olayı tetiklenir.
Girdiğimiz sayıyı alır ve x değişkenine atar.
Eğer x, hedef sayıya eşitse, kullanıcının sayıyı doğru tahmin ettiği anlamına gelir. Bu durumda, kullanıcıya kaç denemede doğru tahmin edildiği gösterilir, textBox1 devre dışı bırakılır ve label3 gizlenir.
Eğer x, hedef sayıdan küçükse, a değeri x + 1 olarak güncellenir ve label1'deki metin değişir. Bu durumda, kullanıcının daha büyük bir sayı girmesi gerektiği bildirilir.
Eğer x, hedef sayıdan büyükse, b değeri x - 1 olarak güncellenir ve label2'deki metin değişir. Bu durumda, kullanıcının daha küçük bir sayı girmesi gerektiği bildirilir.
Kullanıcının tahmin ettiği sayı, hedef sayıya yaklaşık olarak eşit hale gelene kadar bu işlem tekrarlanır.
Tahminlerin sayısı say değişkeniyle takip edilir ve label4'te gösterilir.
Eğer aralık (b - a) 1'den küçük hale gelirse, bu durumda kullanıcının tahmin ettiği sayı, hedef sayıya eşit olmayabilir. Bu durumda, kullanıcıya kaç denemede doğru tahmin edildiği gösterilir, hedef sayı gösterilir, textBox1 devre dışı bırakılır ve label3 gizlenir.
