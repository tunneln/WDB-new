#Web Database (WDB)
####A Semantic Database

##To build WDB run:
UN*X: `$.\build.sh`
Windows: `>build.bat`

##To run WDB on UN*X, do the following:
```
$ cd build/classes
$ export INSTANCE_ROOT="."
$ java -cp "../../lib/je.jar:." wdb.WDB
```

##To run WDB on Windows, do the following:
```
$ cd build/classes
$ export INSTANCE_ROOT="."
$ java -cp "..\..\lib\je.jar;." wdb.WDB
```
