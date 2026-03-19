```
CREATE DATABASE dvd_rental;
USE dvd_rental;

DROP TABLE IF EXISTS borrower;

CREATE TABLE borrower (
    borrower_id INT PRIMARY KEY,
    name VARCHAR(50),
    surname VARCHAR(50),
    address VARCHAR(50),
    status VARCHAR(20)
);
INSERT INTO borrower VALUES
(1, 'Colin', 'Morgan', 'Washington', 'Active'),
(2, 'Bradley', 'James', 'New-York', 'Suspended'),
(3, 'Charlie', 'Puth', 'California', 'Terminated'),
(4, 'Selena', 'Gomez', 'Oregon', 'Active'),
(5, 'Ed', 'Sheeran', 'Florida', 'Active');

SELECT borrower_id AS 'Borrower No', name AS 'Borrower Name', surname AS 'Borrower Surname', address AS 'Borrower Address', status AS 'Borrower Status'
FROM borrower;

SELECT * FROM borrower;
```
