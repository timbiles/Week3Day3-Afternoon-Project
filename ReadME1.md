/_ Table - People _/

/_ Step 1 _/
/_ create table Person (
id integer primary key autoincrement,
Name nvarchar(1000),
Age integer,
Height integer,
City nvarcher(1000),
FavoriteColor nvarchar(1000)
); _/

/_ Step 2 _/
/_ insert into Person(Name, Age, Height, City, FavoriteColor)
values
('Tim Biles', 26, 182, 'Arlington', 'blue'),
('Alissa Biles', 26, 165, 'Arlington', 'green'),
('Olive Biles', 1, 60, 'Arlington', 'no opinion, she is an infant'),
('Kyle Smith', 26, 176, 'Arlington', 'orange'),
('Julie Smith', 27, 170, 'Arlington', 'green'); _/

/_ select _ from person; \*/

/_ Step 3 _/
/_ select _ from person order by height desc; \*/

/_ Step 4 _/
/_ select _ from person order by height; \*/

/_ Step 5 _/
/_ select _ from person order by Age desc; \*/

/_ Step 6 _/
/_ select _ from person where Age > 20; \*/

/_ Step 7 _/
/_ select _ from person where Age = 18; \*/

/_ Step 8 _/
/_ select _ from person where Age < 20 or Age > 30; \*/

/_ Step 9 _/
/_ select _ from person where Age != 27; \*/

/_ Step 10 _/
/_ select _ from person where FavoriteColor != 'red'; \*/

/_ Step 11 _/
/_ select _ from person where FavoriteColor != 'red' and FavoriteColor != 'blue'; \*/

/_ Step 12 _/
/_ select _ from person where FavoriteColor = 'orange' or FavoriteColor = 'green'; \*/

/_ Step 13 _/
/_ select _ from person where FavoriteColor in ('orange', 'green', 'blue'); \*/

/_ Step 14 _/
/_ select _ from person where FavoriteColor in ('yellow', 'purple'); \*/

/_ Table - Orders _/

/_ Step 1 _/
/_ create table Orders(
PersonID integer primary key autoincrement,
ProductName nvarchar,
ProductPrice nvarchar,
Quantity integer
); _/

/_ Step 2 _/
/_ insert into Orders(ProductName, ProductPrice, Quantity)
values
('Shoes', 49.99, 3),
('T-shirt', 9.99, 5); _/

/_ Step 3 _/
/_ select _ from Orders; \*/

/_ Step 4 _/
/_ select sum(Quantity) from Orders; _/

/_ Step 5 _/
/_ select sum(ProductPrice) from Orders; _/

/_ Step 6 _/
/_ select sum(ProductPrice _ Quantity) from Orders where personID = 1; \*/

/_ Table - Artist _/

/_ Step 1 _/
/_ select _ from Artist; \*/

/_ insert into Artist(Name)
values
('Paramore'),
('Muse'),
('Blink 182'); _/

/_ Step 2 _/
/_ select _ from Artist order by name desc limit 10 ; \*/

/_ Step 3 _/
/_ select _ from Artist limit 5; \*/

/_ Step 4 _/
/_ select _ from Artist where Name like 'Black%'; \*/

/_ Step 5 _/
/_ select _ from Artist where Name like '%Black%'; \*/

/_ Table - Employee _/

/_ Step 1 _/
/_ select FirstName, LastName from Employee where City = 'Calgary'; _/

/_ Step 2 _/
/_ select FirstName, LastName, max(BirthDate) from Employee; _/

/_ Step 3 _/
/_ select FirstName, LastName, min(BirthDate) from Employee; _/

/_ Step 4 _/
/_ select _ from Employee; \*/

/_ select FirstName, LastName from Employee where ReportsTo = 2; _/

/_ Step 5 _/
/_ select count(_) from Employee where City = 'Lethbridge'; \*/

/_ Table - Invoice _/

/_ select _ from Invoice; \*/

/_ Step 1 _/
/_ select count(_) from Invoice where BillingCountry = 'USA'; \*/

/_ Step 2 _/
/_ select _, max(Total) from Invoice; \*/

/_ Step 3 _/
/_ select _, min(Total) from Invoice; \*/

/_ Step 4 _/
/_ select _ from Invoice where Total < 5; \*/

/_ Step 5 _/
/_ select count(_) from Invoice where Total < 5; \*/

/_ Step 6 _/
/_ select count(_) from Invoice where BillingState in ('CA', 'TX', 'AZ'); \*/

/_ Step 7 _/
/_ select _ from Invoice; _/
/_ select avg(total) from Invoice; \*/

/_ Step 8 _/
/_ select sum(total) from Invoice; _/
