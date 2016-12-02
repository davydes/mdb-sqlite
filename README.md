[Original Repo](https://code.google.com/archive/p/mdb-sqlite/)

# MS Access to SQLite Converter

## Description

Provides automated conversion of MS Access 2000 databases to SQLite on any platform, utilizing Jackcess and SQLite Java libraries. No native driver required.

MDB-SQLite is used by Plausible Labs to read government-supplied Access databases.

## Usage

To compile, run:

```bash
ant dist
```

This will create a standalone jar in dist/mdb-sqlite.jar

To convert a database file:

```bash
java -jar dist/mdb-sqlite.jar source.mdb output.sqlite
```

### Changes

1.0.2 Release
Prefix index names with the table names to prevent name conflicts when converting indixes.
1.0.1 Release
Work-around around the SQLite JDBC drivers lack of support for boolean values (Issue #2)

Add support for converting indexes (Issue #3)

1.0 Release
Initial Release
