# Labb 1 – SQL Databas för Bokhandel

Detta projekt är en databasdesign för en fiktiv bokhandel, framtagen som del av Labb 1 i SQL-kursen.  
Databasen är uppbyggd med fokus på dataintegritet, rena tabeller och tydliga relationer.

## Databasstruktur

Databasen innehåller följande tabeller:

- **Författare** – information om varje författare (förnamn, efternamn, födelsedatum).
- **Förlag** – information om bokförlag.
- **Butiker** – butikens namn, adress, postnummer och ort.
- **Böcker** – inkluderar titel, ISBN, språk, pris, utgivningsdatum, författare och förlag.
- **LagerSaldo** – hur många exemplar av varje bok som finns i varje butik.
- **Kunder** – kundinformation (förnamn, efternamn, e-post).
- **Ordrar** – kundens beställningar med orderdatum.



##  Testdata

Databasen innehåller:
- 3 butiker
- 4 författare
- 3 förlag
- 10 böcker
- LagerSaldo för samtliga böcker i alla butiker
- 4 kunder
- 4 ordrar


##  Stored Procedure: FlyttaBok

Projektet innehåller en stored procedure för att flytta böcker mellan butiker:


##  Syfte

- Förstå databasdesign
- Arbeta med primärnycklar, främmande nycklar och relationer
- Skriva SQL-skript för att skapa tabeller
- Skriva stored procedures med dataintegritetskontroll
- Hantera testdata för demonstration

---



