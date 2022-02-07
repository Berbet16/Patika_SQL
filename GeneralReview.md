

# Patika_SQL_GENERAL REVIEW QUESTIONS

### Bu çalışmamamızda şimdiye kadar üzerine konuştuğumuz tüm konuları 5 farklı senaryo üzerinden tekrar etmeye çalıştık. Aşağıda ilgili senaryoları bulabilirsiniz.

### film tablosundan 'K' karakteri ile başlayan en uzun ve replacenet_cost u en düşük 4 filmi sıralayınız.

``` SELECT title, replacement_cost,length FROM film WHERE title LIKE 'K%' ORDER BY length DESC, replacement_cost ASC LIMIT 4; ```

### film tablosunda içerisinden en fazla sayıda film bulunduran rating kategorisi hangisidir?

``` SELECT COUNT(*), rating FROM film GROUP BY rating ORDER BY COUNT(*) DESC LIMIT 1; ```

### cutomer tablosunda en çok alışveriş yapan müşterinin adı nedir?

```  SELECT SUM(amount), customer.first_name, customer.last_name FROM payment JOIN customer ON customer.customer_id = payment.customer_id;  ```

### category tablosundan kategori isimlerini ve kategori başına düşen film sayılarını sıralayınız.

```  ```

### film tablosunda isminde en az 4 adet 'e' veya 'E' karakteri bulunan kç tane film vardır?

```  ```
