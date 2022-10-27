 # Shaunda Atkins SQL Portfolio
 ## Welcome to my SQL portfolio! This code repository includes all the code I have written. Please feel free to take a glance and reach out to me via email if you have any questions: satkins619@gmail.com

CREATE TABLE STORE (id INTEGER PRIMARY KEY, name TEXT, quantity INTEGER, price INTEGER, sold INTEGER);

INSERT INTO store VALUES (1, 'Oversized Tunic Sweatshirt for Women', 14, 35.99, 7);
INSERT INTO store VALUES (2, 'Oversized Tunic Sweater for Women', 9, 29.99, 6);
INSERT INTO store VALUEs (3, 'Hooded Sweatshirt for Women', 12, 39.99, 5);
INSERT INTO STORE VALUES (4, 'Cropped Sweatshirt for Women', 10, 34.99, 3);
INSERT INTO STORE VALUES (5, 'Water-Resistant Raincoat for Women', 12, 49.99, 5);
INSERT INTO STORE VALUES (6, 'Oversized Sherpa Overcoat for Women', 13, 44.99, 6);
INSERT INTO STORE VALUES (7, 'Double-Breasted Hooded Wool Peacoat for Women', 8, 89.99, 3);
INSERT INTO STORE VALUES (8, 'Long Open-Front Sweater for Women', 13, 32.99, 5);
INSERT INTO STORE VALUES (9, 'Button-up Round Neck Sweater for Women', 14, 29.99, 6);
INSERT INTO STORE VALUES (10, 'Frayed Fleece Scarf', 15, 12.99, 6);
INSERT INTO STORE VALUES (11, 'Knitted Fleece Beanie', 14, 11.99, 9);
INSERT INTO STORE VALUES (12, 'Fleece Glove', 13, 9.99, 5);

-----Display the store database in order by price.
SELECT * FROM STORE order by price asc;

----What is the total amount sold in the store from items in the database?
SELECT SUM (PRICE) FROM STORE;

----What is the total quantity of items sold in the store from the items in the database?
SELECT SUM (SOLD) FROM STORE;

-----Which item had the most items sold in the store?
select name,sold from store order by sold desc

