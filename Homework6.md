# Patika_SQL_Homework6

### film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?

``` SELECT AVG(rental_rate) FROM film; ```

### film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?

``` SELECT COUNT(*) FROM film WHERE film LIKE '%c'; ```

### film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?

``` SELECT COUNT(title) FROM film WHERE title LIKE 'T%' AND rating = 'G'; ```

### film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?

``` SELECT COUNT(country) FROM country WHERE country LIKE '_____'; ```
