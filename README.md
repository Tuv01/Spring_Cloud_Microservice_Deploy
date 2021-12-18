# Final Project: Web Development with Java Spring Framework
## by Peter the Great St. Petersburg Polytechnic University

### The task is to develop of RESTFull Web Services with Spring MVC and Hibernate CRUD on an arbitrary topic:
library of books

movie library

storage of audio files

hockey standings

tennis standings

etc.

### Technology stack: java 8, Spring 5, flyway, hibernate, maven, PostgreSQL/MySQL..

The topic chosen for this project is the library of books and for this purpose I have used the database proposed in the following link:<br/><br/>
https://www.pluralsight.com/guides/querying-data-with-sql-dql <br/><br/>
Database Information:  <br/><br/>
authors, publishers, customers, and librarians: unique identifiers for each record and the corresponding names. <br/><br/>

books: besides the unique identifier for each book and its name, books also have a 13-character ISBN, an edition number, and are related to an author and publisher through the use of foreign keys. As such, they point to the unique identifiers from those tables, thus ensuring that the author and publisher of a given book already exists in the database.
The unique identifiers in the above tables act as primary keys. Particularly, in the books table, we are not using the ISBN for that purpose since we may have multiple copies of the same book and edition.<br/><br/>

loans stores each book loan that has been made. The use of author_id, customer_id, and book_id as foreign keys are complemented by the loan date and current status (active or not).<br/><br/>

