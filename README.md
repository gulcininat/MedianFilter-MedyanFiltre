# Median Filter - Medyan Filtre
Applying a median filter on an image 

// Bir görsel üzerinde medyan filtre uygulaması

Matlab programında kayıtlı olan Cameraman.tif görüntüsü üzerinde medyan filtre uygulamasıdır. 
4. satırdaki kodda, sizin kendi bilgisayarınızda kayıtlı olan görüntünün adresini ve ismini kullanarak aynı uygulamayı yapabilirsiniz.
Bunun için 3. satırı kapatıp, 4. satırı açmanız ve uzantıyı değiştirmeniz yeterli olacaktır.

    Median (Medyan) Filtre

Yukarıda, medyan filtre uygulamasının matlab kodu verilmiştir. Kodda, öncelikle yüklenen resmin gri seviye görüntü değil ise, gri seviyeye dönüştürme işlemi yapılmıştır. Daha sonra 3x3 lük bir filtre gezdirilerek görüntüdeki her piksel değeri için, öncelikle alt üst ve çapraz komşuları ile kendisi bir diziye atılarak küçükten büyüğe sıralanmış ve ortadaki değeri yani 5. değeri (3x3 filtrede 9 piksel olduğu için) yeni piksel değeri olarak atanmıştır. Bu işlem her piksel için ayrı ayrı komşuları arasından medyan değerlerini bulup, yeni piksel değeri olarak atanarak gerçekleştirilmiştir. Medyan filtresi, doğrusal olmayan bir filtredir. Tuz&Biber gürültüsünde, ortalama filtreden çok daha iyi sonuçlar vermektedir. Son olarak, görüntünün boyutunda azalma olduğundan dolayı ilk görüntünün, ilk ve son satırı ile ilk ve son sütunu da filtreden geçmiş görüntüye eklenir. Böylece boyut kaybı yaşanmamış olur.

Kodun çalıştırıldığında:
Solda orijinal görüntü, sağda ise medyan filtre uygulanmış hali bulunmaktadır. 
