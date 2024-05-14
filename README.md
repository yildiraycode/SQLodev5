# SQLodev5
## sql sorguları patika odev 5 ##
**Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.**<br/>
1.film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.<br/><br/>
SELECT title from film<br/>
WHERE title LIKE '%n' <br/>
ORDER BY length<br/>
LIMIT 5;<br/><br/><br/>
2.film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.<br/><br/>
SELECT title from film<br/>
WHERE title LIKE '%n' <br/>
ORDER BY length DESC<br/>
OFFSET 5<br/>
LIMIT 5;<br/><br/><br/>
3.customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.<br/><br/>
SELECT * from customer<br/>
where store_id=1<br/>
order by last_name desc<br/>
LIMIT 4;<br/><br/>
