#Web Database (WDB)

###What is WDB?
WDB is a semantic database management system developed by Dr. Phil Cannata and Bo Li. WDB is based on the Semantic Information Manager (SIM) and semantic data model developed by Doug Tolbert. The purpose of the database was to more accurately capture the meaning of the data and it's relationships so that the Schema better represents the corresonding real world objects.
###What is WDB-new?
WDB-new is my re-implementation of the WDB system on top of Oracle NoSQL DB. WDB was originally implemented on top of [Berkley DB JE](https://blogs.oracle.com/charlesLamb/entry/oracle_nosql_database_vs_berkeley) - an embedded database for key/value stores intially developed by Sleepycat.

###To build WDB run:
On UN*X: `$.\build.sh`

On Windows: `>build.bat`



###To run WDB, do the following:
**On UN*X:**
```
$ cd build/classes
$ export INSTANCE_ROOT="."
$ java -cp "../../lib/je.jar:." wdb.WDB
```
**On Windows:**
```
$ cd build/classes
$ export INSTANCE_ROOT="."
$ java -cp "..\..\lib\je.jar;." wdb.WDB
```



###More on WDB
WDB's higher-level database model enables the database designer and the users to see a conceptual view of the database. A benefit of this in practice is that the schema is able to capture nearly all of the semantics of the database. This essentially allows one to go **directly** from the Conceptual Model to a Schema, as opposed to the fiasco of having to go from a Conceptual to Logical to Physical Model *and then* to a Schema, as you would with a relational database. This benefit also brings with it optimizations to queries, such as never having to JOIN tables, since the relationships are already defined within the schema itself.

Even more on WDB can be found [here](http://www.cs.utexas.edu/~cannata/dbms/web-pages/Class%20Notes/02%20Data%20Models/Bo%20Li%20Thesis.pdf) 
