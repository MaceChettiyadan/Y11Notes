- **Data** - facts and figures - it is raw information
	- We create tables - primitive forms are spreadsheets

### RDBMS
- To create data redundancy, and reduce data anomalies
- An ID is the first step to achieving data reliability

##### Normalisation
- **Data Normalisation** is the splitting of one table into multiple tables to separate key dependencies
	- This is so that in an *Appointments* table, for example, we can use a foreign key *DoctorID* instead of storing all of the doctor's details
- $1^{st}NF$
	- Primary Key - unique and not null or empty
	- If it does not have a 1stNF it is non-normalised data
- $2^{nd}NF$
	- You split data into multiple tables based on key dependencies
	- For example, in an *items* table, there can be a field for supplier and department
		- Yet, Item, Department and Supplier are all separate entities
		- 

**ERD/DFD entities**
![[Table-Entity.svg|size=50px]]
- you will get backstabbed ? if you are a chef you will get shot ?
