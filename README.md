# Patika.dev SQL Task-2
 ### dvdrental örnek veri tabanı kullanılmıştır <br>
 _tablolara sqltask2.1.csv şeklindeki başlıklardan ulaşabilirsiniz_

1. **film** tablosunda bulunan tüm sütunlardaki verileri replacement cost değeri 12.99 dan büyük eşit ve 16.99 küçük olma koşuluyla sıralayınız ( BETWEEN - AND yapısını kullanınız.)
2. .**actor** tablosunda bulunan first_name ve last_name sütunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' değerleri olması koşuluyla sıralayınız. ( IN operatörünü kullanınız.)
3. **film** tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99, 2.99, 4.99 **VE** replacement_cost 12.99, 15.99, 28.99 olma koşullarıyla sıralayınız. ( IN operatörünü kullanınız.)



1. ```sql
   select * from film 
   where replacement_cost between 12.99 and 16.99;
   ```

2. ```sql
   select * from actor 
   where first_name IN ('Penelope', 'Nick', 'Ed');
   ```

3. ```sql
   select * from film
   where (rental_rate in ('0.99', '2.99', '4.99')) and (replacement_cost in ('12.99', '15.99', '28.99'));
   ```

   
