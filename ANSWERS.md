## MAIN QUESTIONS

1. SELECT all the data FROM the artist table.
```SQL
SELECT * FROM artist;
```
2. SELECT the first_name, last_name, and country FROM the employee table
```SQL
SELECT first_name, last_name, country FROM employee;
```
3. SELECT the name, composer, and milliseconds FROM the track table WHERE the milliseconds are greater than 299000.
```SQL
SELECT name, composer, milliseconds
FROM track
WHERE milliseconds > 299000;
```
4. SELECT the count FROM the track table WHERE the milliseconds are greater than 299000.
```SQL
SELECT count(*)
FROM track
WHERE milliseconds > 299000;
```

## BLACK DIAMOND

1. Find the average length of all tracks in milliseconds
```SQL
SELECT avg(milliseconds) FROM track;
```
2. Find the number of invoices in the USA
```SQL
SELECT count(*) FROM invoice;
```
3. Make a list of all the First Names of Customers that contain an 'a'
```SQL
SELECT first_name FROM customer
WHERE first_name LIKE '%a%';
```
4. Make a list of the 10 longest tracks
```SQL
SELECT * FROM track
ORDER BY milliseconds DESC
LIMIT 10;
```
5. Make a list of the 20 shortest tracks
```SQL
SELECT * FROM track
ORDER BY milliseconds
LIMIT 20;
```
6. Find all the customers that live in California or Washington
```SQL
SELECT * FROM customer
WHERE state IN ('CA', 'WA');
```
7. Find all the customers that live in California, Washington, Utah, Florida, or Arizona (Use IN keyword)
```SQL
SELECT * FROM customer
WHERE state IN ('CA', 'WA', 'UT', 'FL', 'AZ');
```
8. Insert an artist to the database
```SQL
INSERT INTO artist
(name)
VALUES
('John Mayer');
```
9. Insert yourself as a customer to the database
```SQL
INSERT INTO customer
(address, city, state, country, postal_code, phone, fax, email, last_name, first_name)
VALUES
('My Address', 'Dallas', 'TX', 'US', '75201', '214-123-1234', 'lul who faxes?', 'my@email.com', 'Palmer', 'Jeff');
```
10. Find a list of all Playlists that start with Classical
```SQL
SELECT * FROM playlist
WHERE name LIKE 'Classical%';
```

