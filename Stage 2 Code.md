```
CREATE DATABASE dvd_rental;
USE dvd_rental;

DROP TABLE IF EXISTS borrower;
DROP TABLE IF EXISTS dvd;

CREATE TABLE borrower (
    borrower_id INT PRIMARY KEY,
    name VARCHAR(50),
    surname VARCHAR(50),
    address VARCHAR(50),
    status VARCHAR(20)
);

CREATE TABLE dvd (
    dvd_id INT PRIMARY KEY,
    title VARCHAR(50),
    category VARCHAR(50),
    year INT,
    rental_cost DECIMAL(5,2)
);

INSERT INTO borrower VALUES
(1, 'Colin', 'Morgan', 'Washington', 'Active'),
(2, 'Bradley', 'James', 'New-York', 'Suspended'),
(3, 'Charlie', 'Puth', 'California', 'Terminated'),
(4, 'Selena', 'Gomez', 'Oregon', 'Active'),
(5, 'Ed', 'Sheeran', 'Florida', 'Active');

INSERT INTO dvd VALUES
(11, 'Subway', 'Action', 2012, 4.40),
(12, 'Brownie', 'Comedy', 2016, 4.05),
(13, 'Harry Potter', 'Action', 2002, 3.70),
(14, 'Guardians of the Galaxy', 'Action', 2014, 3.95);

SELECT borrower_id AS 'Borrower No', name AS 'Borrower Name', surname AS 'Borrower Surname', address AS 'Borrower Address', status AS 'Borrower Status'
FROM borrower;

SELECT dvd_id AS 'DVD ID', title AS 'Title', category AS 'Category', year AS 'year', rental_cost AS 'Rental Cost'
FROM dvd;

SELECT * FROM borrower;
SELECT * FROM dvd; 
```
