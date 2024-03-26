# SQL_Assignment_3

## Sorgu Senaryoları

* Country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.


```bash
SELECT country
FROM country
WHERE country LIKE 'A%a';
```

* Country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.

```bash
SELECT country
FROM country
WHERE LENGTH(country) >= 6
AND country LIKE '%n';
```

* Film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.

```bash
SELECT title
FROM film
WHERE LOWER(title) LIKE '%t%'
AND LENGTH(title) >= 4;
```

