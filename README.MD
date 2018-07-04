/_ CREATE TABLE Person (
ID INTEGER PRIMARY KEY AUTOINCREMENT,
Name string,
Age integer,
Height integer,
City string,
FavoriteColor string
); _/

/_ SELECT _ FROM Person \*/

/_ INSERT INTO Person (Name, Age, Height, City, FavoriteColor)
VALUES(
"Jim Bo",
22,
60,
"Seattle",
"Red"
);
_/

/_ INSERT INTO Person (Name, Age, Height, City, FavoriteColor)
VALUES(
"Blee bloo",
34,
293,
"Gorka-Morka",
"Purple"
);
_/
/_ INSERT INTO Person (Name, Age, Height, City, FavoriteColor)
VALUES(
"Glib Glob",
50,
274,
"Boston",
"Blue"
); _/

/_ INSERT INTO Person (Name, Age, Height, City, FavoriteColor)
VALUES(
"Dennis Rodman",
50,
1284,
"New York",
"All of them"
); _/

/_ INSERT INTO Person (Name, Age, Height, City, FavoriteColor)
VALUES(
"Michael Jackons",
60,
456,
"Never Land",
"Gold"
); _/

/_ SELECT _ FROM Person ORDER BY Height desc; \*/

/_ SELECT _ FROM Person ORDER BY Height; \*/

/_ SELECT _ FROM Person ORDER BY Age desc; _/

/_ SELECT _ FROM Person WHERE Age >20; _/

/_ SELECT _ FROM Person WHERE Age = 18; \*/

/_ SELECT _ FROM Person WHERE Age <20 OR Age >30; \*/

/_ SELECT _ FROM Person WHERE Age != 27; \*/

/_ SELECT _ FROM Person WHERE FavoriteColor != "Red" \*/

/_ SELECT _ FROM Person WHERE FavoriteColor != "Red" AND FavoriteColor != "Blue";
\*/

/_ SELECT _ FROM Person Where FavoriteColor = "Orange" OR FavoriteColor = "Green"; \*/

/_ SELECT _ FROM Person WHERE FavoriteColor IN ("Orange","Green","Blue"); _/
/_ SELECT _ FROM Person WHERE FavoriteColor IN ("Yellow","Purple") _/

/_///////////////////////////////////////////////////////////////////////////////////////////////// _/

/_ CREATE TABLE Orders (
PersonID integer ,
ProductName string,
ProductPrice float,
Quantity integer
)
_/

/_ INSERT INTO Orders (PersonID, ProductName, ProductPrice, Quantity)
VALUES(
1,
"Bats",
100.25,
25
)
_/

/_ INSERT INTO Orders (PersonID, ProductName, ProductPrice, Quantity)
VALUES(
2,
"Bread",
24.95,
6
); _/

/_ INSERT INTO Orders (PersonID, ProductName, ProductPrice, Quantity)
VALUES(
3,
"Beets",
6.34,
100
); _/

/_ INSERT INTO Orders (PersonID, ProductName, ProductPrice, Quantity)
VALUES(
4,
"BSG",
25.98,
1
); _/

/_ INSERT INTO Orders (PersonID, ProductName, ProductPrice, Quantity)
VALUES(
5,
"cans",
2.50,
29
); _/

/_ SELECT _ FROM Orders; \*/

/_ SELECT SUM(Quantity) FROM Orders _/

/_ SELECT SUM(ProductPrice _ Quantity) FROM Orders \*/

/_ SELECT SUM (ProductPrice _ Quantity) FROM Orders WHERE PersonID = 2; \*/

/_ SELECT _ FROM Employee \*/

/_ SELECT FirstName, LastName FROM Employee WHERE City = "Calgary" ; _/

/_ SELECT FirstName, LastName, MAX(BirthDate) FROM Employee _/

/_ SELECT FirstName, LastName, MIN(BirthDate) FROM Employee _/

/_ SELECT _ FROM Employee WHERE ReportsTo = 2; \*/

/_ SELECT COUNT(_) FROM Employee WHERE City = "Lethbridge" \*/

/_ ///////////////////////////////////////////////////////////////////////////////////// _/

/_ SELECT COUNT(_) FROM Invoice WHERE BillingCountry = 'USA'; \*/

/_ SELECT MAX(TOTAL) FROM Invoice _/

/_ SELECT MIN(TOTAL) FROM Invoice _/

/_ SELECT _ FROM Invoice WHERE Total < 5 \*/

/_ SELECT COUNT(_) FROM Invoice WHERE Total < 5 \*/

/_ SELECT COUNT(_) FROM Invoice WHERE BillingState IN ("CA","TX","AZ") \*/

/_ SELECT AVG(Total) FROM Invoice; _/

/_ SELECT SUM(Total) FROM Invoice; _/
