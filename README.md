# SQL
Comando de sql

--between
SELECT *
FROM Production.Product
WHERE ListPrice NOT between 1000 and 1500;

SELECT * 
FROM HumanResources.Employee
WHERE HireDate between '2009/01/01' and '2010/01/01'
order by HireDate

--IN

SELECT * 
FROM Person.Person
WHERE BusinessEntityID not in (2,7,13)

--LIKE

SELECT *
FROM Person.Person
WHERE FirstName like 'ovi%'


SELECT * 
FROM Person.Person
WHERE FirstName like '%essa%'
------------------------------------------

SELECT COUNT (ListPrice)
FROM Production.Product
WHERE ListPrice > 1500


SELECT COUNT (LastName)
FROM Person.Person
WHERE LastName LIKE 'P%'


SELECT COUNT (DISTINCT City)
FROM Person.Address


SELECT DISTINCT (city)
FROM Person.Address
order by City asc

SELECT COUNT (*)
FROM Production.Product
WHERE color = 'RED' 
and ListPrice BETWEEN 500 and 1000

SELECT COUNT( * )
FROM Production.Product
WHERE Name LIKE '%road%'
