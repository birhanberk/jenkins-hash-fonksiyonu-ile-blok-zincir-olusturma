## Hakkında

* Girdi olarak bulunduğu dizindeki 001.txt dosyasını alır ve çıktı olarak 32 bitlik bir özet değeri oluşturur.
* Bir dosya için her çalıştırılmasında aynı değeri üretmektedir.
* Dosyadaki küçük bir değişiklik özet değerinde tahmin edilemeyecek bir değişikliğe neden olmaktadır.

## Yapı

İlk blok içerisinde 001.txt dosyasındaki text yer alır. Sıradaki her bir blok kendinden önceki bloğun özet değeri ve rastgele 32 bitlik bir sayı ile elde edilir. Bu bloğun ilk 8 biti sıfırlardan oluşur. Özet alma işlemi için Jenkins hash fonksiyonu kullanılmıştır. Program çalışmaya başladığında bulunduğu dizinde yer alan 001.txt dosyasından 100.txt dosyasına kadar 99 dosya oluşturur ve oluşturulan özet değerler bu dosyalarda yer alır. HASHSUM isimli dosyaya her blok oluşturulurken eklenen rastgele sayı ve bloğun özet değeri yazdırılır. Program çalışma süresi 10 dakikadır. Bu süre boyunca dosyalar oluşturulamamış olsa bile program sonlanmaktır.
