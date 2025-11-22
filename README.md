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

Alla relationer skapas med **foreign keys**, och databasen använder **INT** för datum samt **NVARCHAR(255)** för alla textfält.

##  Testdata

Databasen innehåller:
- 3 butiker
- 4 författare
- 3 förlag
- 10 böcker
- LagerSaldo för samtliga böcker i alla butiker
- 4 kunder
- 4 ordrar

Testdatan används för att demonstrera funktionalitet och för att kunna testa stored procedures och SELECT-satser.

##  Stored Procedure: FlyttaBok

Projektet innehåller en stored procedure för att flytta böcker mellan butiker:

Proceduren:
- Kontrollerar att från-butiken har tillräckligt antal
- Flyttar antal exemplar mellan butiker
- Använder **transaktioner** för att skydda dataintegritet
- Gör ROLLBACK om något går fel

##  Syfte

- Förstå databasdesign
- Arbeta med primärnycklar, främmande nycklar och relationer
- Skriva SQL-skript för att skapa tabeller
- Skriva stored procedures med dataintegritetskontroll
- Hantera testdata för demonstration

---



