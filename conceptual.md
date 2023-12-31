### Conceptual Exercise

Answer the following questions below:

- What is PostgreSQL?
PostgreSQL is an open-source relational database management system (RDBMS) that is known for its extensibility, standards compliance, and robustness. It supports a wide range of data types and has advanced features such as transactions, concurrency control, and foreign keys. PostgreSQL is often used for large-scale, complex applications and is known for its reliability and extensibility.

- What is the difference between SQL and PostgreSQL?
SQL (Structured Query Language) is a standardized language for managing and manipulating relational databases. PostgreSQL, on the other hand, is a specific implementation of an RDBMS that uses SQL as its query language. In other words, SQL is a language, while PostgreSQL is a database management system that uses SQL.
- In `psql`, how do you connect to a database?
psql -U username -d database_name -h host -p port

- What is the difference between `HAVING` and `WHERE`?
The WHERE clause is used in SQL to filter rows before they are grouped and aggregated, while the HAVING clause is used to filter the results of aggregate functions after the grouping has occurred. In simple terms, WHERE filters individual rows, and HAVING filters grouped results.

- What is the difference between an `INNER` and `OUTER` join?
An INNER JOIN returns only the rows that have matching values in both tables, excluding non-matching rows. An OUTER JOIN (or simply LEFT OUTER JOIN or RIGHT OUTER JOIN) returns all rows from one table and the matching rows from the other. Non-matching rows from the second table will contain NULL values.

- What is the difference between a `LEFT OUTER` and `RIGHT OUTER` join?
In a LEFT OUTER JOIN, all rows from the left table and the matching rows from the right table are returned. In a RIGHT OUTER JOIN, all rows from the right table and the matching rows from the left table are returned. The key distinction is which table's all rows are included in the result.

- What is an ORM? What do they do?
An ORM (Object-Relational Mapping) is a programming technique that allows data to be accessed and manipulated using an object-oriented paradigm. It maps objects to database tables, abstracting away the need for direct SQL queries. ORMs provide a higher-level, more intuitive interface for developers to interact with databases.

- What are some differences between making HTTP requests using AJAX 
  and from the server side using a library like `requests`?
  AJAX (Asynchronous JavaScript and XML) is a client-side technology that allows web pages to be updated asynchronously by exchanging small amounts of data with the server. On the server side, using a library like requests in a programming language (e.g., Python) allows the server to make HTTP requests to other servers. The key difference is the origin of the request: AJAX is initiated by the client, while server-side requests are initiated by the server.

- What is CSRF? What is the purpose of the CSRF token?
CSRF (Cross-Site Request Forgery) is a type of web security vulnerability where an attacker tricks a user's browser into making an unintended request. A CSRF token is a security measure used to mitigate this vulnerability. The token is included in requests, and the server verifies its presence to ensure that the request is legitimate and not forged by a malicious third party.

- What is the purpose of `form.hidden_tag()`?
In web development with frameworks like Flask, form.hidden_tag() is used to include hidden fields in HTML forms that contain a security token. This token helps prevent CSRF attacks by ensuring that the form submission originated from the same application and was not tampered with by a malicious actor. The hidden fields are typically used to store the CSRF token and other necessary information.