# Patika_SQL_Homework4

### film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.

```  ```

### film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.

``` SELECT COUNT(DISTINCT replacement_cost) FROM film; ```

### customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?

``` SELECT COUNT(title) FROM film WHERE title LIKE 'T%' AND rating = 'G'; ```

### city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.

``` SELECT COUNT(country) FROM country WHERE country LIKE '_____'; ```


