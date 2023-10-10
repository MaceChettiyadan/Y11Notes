## Databases
### relationship between data and information
- There is a **distinction** between data and information. 
	- **Data** is made up of raw <mark style="background: #ADCCFFA6;">facts and figures</mark>. It is a form of raw information;
	- That is, **Information** is data that has been <mark style="background: #ADCCFFA6;">analysed and interpreted</mark> to produce meaning.

### flat file vs relational database
- A **flat file** database is a <mark style="background: #ADCCFFA6;">two-dimensional singular table</mark> database made up of rows of data. It has no relationships between each datum. The most common flat file format is in the **CSV** (Comma separated values) format.
- A **relational** database is made up of multiple tables (entities) that contain records and have multiple fields/attributes. Relational databases, as the name suggests, <mark style="background: #ADCCFFA6;">have relationships between pieces of data</mark> through the use of <mark style="background: #ADCCFFA6;">unique identifiers called keys</mark>.

### relational database management systems (RDBMS):
#### role of a RDBMS in handling access to data
- An RDBMS provides secure and efficient storage and access to data through features such as data integrity, data security, performance optimisation and data security.

#### independence of data from RDBMS
- data independence from an RDBMS is the **capability for the database structure to be modified without having to rewrite or modify any applications that depend on the database**; while the RDBMS is an interface (API) for modification of the database, it still <mark style="background: #ADCCFFA6;">exists independently of the RDBMS</mark>.

### organisation of a relational database
#### entities
- An entity is a real object/thing that exists in the physical world and is a logical construct.
#### attributes
- attributes belong to tables, and may also be called fields. they describe the different properties of the table, translated from the logically constructed entity.
#### relationships
- **1:1** one to one relationships have each field of an entity <mark style="background: #ADCCFFA6;">related to only one field</mark> of another, and **vice versa**
- **1:M** one to many relationships have each field of an entity <mark style="background: #ADCCFFA6;">related to potentially multiple fields</mark> in another entity, but **not vice versa**
- **M:M** many to many relationships have each field of an entity <mark style="background: #ADCCFFA6;">related to potentially multiple fields</mark> in another entity, and **vice versa**
	- these relationships are frowned upon because they create unwanted data redundancy and reduce data integrity through the introduction of insert, update and delete anomalies.
#### tables as the implementation of entities, consisting of fields and records
- in order to translate the logical construct that is an entity and thus implement a real object/thing into a database, tables are used. fields/attributes are the properties of the entity, and records describe each point of data.

#### hierarchical structure of data
- tables have records have fields.

#### datatypes
- **date:** represented in most SQL standards as `Date`, can specify a format default but it is usually YYYY-MM-DD
- **text:** use `Text` or `Char` - char is obviously a lot shorter, both have sizes, char is to 255 and text is basically anything in practice.
- **int:** signed or unsigned `INT` has a size.
- **float:** most sql servers determine whether to use float or double automatically so just use `FLOAT`
- **boolean:** `Bool` **importantly,** it is a numeric value with zero false 1 true.

### primary and foreign keys to link tables
- Primary keys are the unique identifiers and are used by foreign keys to establish secure, integral relations between data

### composite key
- a primary key is not only one column. it is a **big misconception**
	- there is <mark style="background: #ADCCFFA6;">ONLY ONE PRIMARY KEY **that may be made up of MULTIPLE COLUMNS**</mark>
- when there are multiple columns it is a **composite key**

### data anomalies
- insert, update and delete anomalies. 
- they are most often caused by unwanted data redundancy (repetition).
- they can be resolved through normalisation
	- **insert:** in a flat file database, it may not be possible to insert data without redundantly repeating other data, or adding another unrelated data point; for example in a library flat file, a patron may require a book to be added. this may not always be possible so is anomalous
	- **update:** if there exist multiple redundant copies of data such as in a flat file, if the data is to be updated and any instance is not updated, then 'zombie' data that is different from what it should be remains
	- **delete:** if the deletion of unwanted information leads to the deletion of desired information there is an anomaly. this is particularly evident in a flat file. also if there is redundant data, then all instances must be deleted.

### purpose of database documentation for developers
- the purpose of database documentation for developers is to communicate the logical design of the database to achieve the most efficient storage and relationships between data in an RDBMS, and thus reduce redundancy and thus data anomalies.

### factors influencing integrity of data, including:
#### currency
- refers to how **up-to-date** data is, including frequency of data updates and latency of updating systems
#### authenticity
- refers to the genuineness of the data, ensuring it accurately represents information it's supposed to depict.
#### relevance
- refers to whether the data is relevant to the database and has a purpose within it
#### accuracy
- refers to the extent to which the data measures what its trying to measure (physics reference)
#### outliers (cleaning)
- outliers that skew data and are obviously not appropriate for the database should be cleaned, whether that be through mathematical distribution or outright removal




### Ethical Issues
#### collecting data about individuals
- Privacy Act 1988. You must have **written consent** to collect the data
#### privacy concerns
- SQL Injection!!! Deletion of data for the company, exposure for customers, modification of data.
#### appropriate use of data
- data mining, how are you goi ng to use data. dont store old data.

### Security Issues
#### Keeping personal data private
- Encryption, privileges
#### backups of organisational data
- RAID independent array of disks.
#### restricting access to data
- access cards, privileges - physical and digital


