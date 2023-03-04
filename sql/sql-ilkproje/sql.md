# -ODEV1-SQL
DVDRENTAL SORGU SENARYOLARI ÇÖZÜMLERİ
Sorgu 1- film tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.
Çözüm 1- SELECT title, description FROM film;
<img width="910" alt="Ekran Resmi 2023-03-01 14 38 08" src="https://user-images.githubusercontent.com/116847744/222129117-6c6022a9-5af2-4927-b7d7-96439af2165d.png">

Sorgu 2- film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük VE 75 ten küçük olma koşullarıyla sıralayınız.
Çözüm 2- SELECT * FROM film 
WHERE length > 60 
AND length < 75;
<img width="715" alt="Ekran Resmi 2023-03-01 15 03 50" src="https://user-images.githubusercontent.com/116847744/222134370-d6b5db37-7df5-42e5-80d8-aab018ae681a.png">

Sorgu 3- film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarıyla sıralayınız.
Çözüm 3- SELECT * FROM film 
WHERE (rental_rate = 0.99) 
AND (replacement_cost = 12.99 OR replacement_cost = 28.99); 
<img width="594" alt="Ekran Resmi 2023-03-01 14 56 04" src="https://user-images.githubusercontent.com/116847744/222132691-5a705157-2cbe-45d8-bfb1-6f61a7628a59.png">

Sorgu 4- customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?
Çözüm 4- SELECT first_name, last_name FROM customer 
WHERE first_name = 'Mary';
<img width="715" alt="Ekran Resmi 2023-03-01 14 57 53" src="https://user-images.githubusercontent.com/116847744/222133080-dc66906b-e523-41bd-a1fc-976d78ef9236.png">

Sorgu 5- film tablosundaki uzunluğu(length) 50 ten büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 veya 4.99 OLMAYAN verileri sıralayınız.
Çözüm 5- SELECT length, rental_rate FROM film 
WHERE length < 50 
AND (rental_rate <> 2.99 AND rental_rate <> 4.99);
<img width="708" alt="Ekran Resmi 2023-03-01 15 00 59" src="https://user-images.githubusercontent.com/116847744/222133772-6c420b19-fb0f-4f66-aba0-33db4b441760.png">

