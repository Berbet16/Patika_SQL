# Patika_SQL_Homework8

### 1. test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

``` CREATE TABLE employee 
(id INT PRIMARY KEY,
 name VARCHAR(50) NOT NULL,
 birthday DATE,
 email VARCHAR(100) NOT NULL
);
```

### 2. Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

```
insert into employee (id, name, birthday, email) values (11, 'Alberto Rowbottam', '1982-06-25', 'arowbottama@wordpress.org');
insert into employee (id, name, birthday, email) values (12, 'Borden Lanaway', '1912-09-02', 'blanawayb@vimeo.com');
insert into employee (id, name, birthday, email) values (13, 'Donnie Wrack', '1925-11-22', 'dwrackc@cmu.edu');
insert into employee (id, name, birthday, email) values (14, 'Grazia Jerams', '1980-07-14', 'gjeramsd@nifty.com');
insert into employee (id, name, birthday, email) values (15, 'Harlie Meegin', '1971-03-12', 'hmeegine@theguardian.com');
insert into employee (id, name, birthday, email) values (16, 'Dorolice Tuftin', '1932-03-20', 'dtuftinf@so-net.ne.jp');
insert into employee (id, name, birthday, email) values (17, 'Hildegarde Pude', '1949-04-05', 'hpudeg@google.com.hk');
insert into employee (id, name, birthday, email) values (18, 'Brendis Ambresin', '1909-02-24', 'bambresinh@nymag.com');
insert into employee (id, name, birthday, email) values (19, 'Theodosia Divers', '1904-03-17', 'tdiversi@storify.com');
insert into employee (id, name, birthday, email) values (20, 'Sybilla Frany', '1913-05-28', 'sfranyj@ovh.net');
insert into employee (id, name, birthday, email) values (21, 'Billye Fordham', '1923-07-22', 'bfordhamk@netlog.com');
insert into employee (id, name, birthday, email) values (22, 'Hashim Pulham', '1966-07-23', 'hpulhaml@nyu.edu'); 
insert into employee (id, name, email, birthday) values (1, 'Frederick', 'fbaszniak0@myspace.com', '2010-06-11');
insert into employee (id, name, email, birthday) values (2, 'Tonia', 'tpedrick1@webnode.com', '2000-12-30');
insert into employee (id, name, email, birthday) values (3, 'Gerry', 'gkamiyama2@digg.com', '2013-12-29');
insert into employee (id, name, email, birthday) values (4, 'Alyce', 'agreenway3@uiuc.edu', '2016-12-21');
``` 

### 3. Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

```
UPDATE employee
SET name = 'Veli'
WHERE id = 1;

UPDATE employee
SET email = 'tonia@tonia24.com'
WHERE name = 'Tonia';

UPDATE employee
SET name = 'Mehmet'
WHERE birthday = '2000-08-12';

UPDATE employee
SET birthday = '1999-10-23'
WHERE email LIKE 'ag%';

UPDATE employee
SET email = 'test@gmail.com'
WHERE id = 7;
```

### Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

```
DELETE FROM employee
WHERE id = 14;

DELETE FROM employee
WHERE birthday = '1935-08-12';

DELETE FROM employee
WHERE name = 'Veli';

DELETE FROM employee
WHERE id IN (18, 19, 12);

DELETE FROM employee
WHERE email = 'agreenway3@uiuc.edu';
```


