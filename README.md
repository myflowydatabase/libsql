


# What is libSQL?

[libSQL]() is an open source, open contribution fork of SQLite. We aim to evolve it to suit many more use cases than SQLite was originally designed for, and plan to use third-party OSS code wherever it makes sense.

libSQL is licensed under an [Open Source License](LICENSE.md), and we adhere to a clear [Code of Conduct](CODE_OF_CONDUCT.md)

## Why a fork?

SQLite has solidified its place in modern technology stacks, embedded in nearly any computing device you can think of. Its open source nature and public domain availability make it a popular choice for modification to meet specific use cases.

But despite having its code available, SQLite famously doesn't accept external contributors and doesn't adhere to a code of conduct. So community improvements cannot be widely enjoyed.

There have been other forks in the past, but they all focus on a specific technical difference. We aim to be a community where people can contribute from many different angles and motivations.

We want to see a world where everyone can benefit from all of the great ideas and hard work that the SQLite community contributes back to the codebase. Community contributions work well, because we’ve done it before. If this was possible, what do you think SQLite could become?

You can read more about our goals an motivation in our [product vision]().

## Compatibility with SQLite

Compatibility with SQLite is of great importance for us. But it can mean many things. So here's our stance:

* **The file format**: libSQL will always be able to ingest and write the SQLite file format. We would love to add extensions like encryption, and CRC that require the file to be changed. But we commit to always doing so in a way that generates standard sqlite files if those features are not used.
* **The API**: libSQL will keep 100% compatibility with the SQLite API, but we may add additional APIs.
* **Embedded**: SQLite is an embedded database that can be consumed as a single .c file with its accompanying header. libSQL will always be embeddable, meaning it runs inside your process without needing a network connection. But we may change the distribution, so that object files are generated, instead of a single .c file.

## Quickstart

```
./configure && make
./libsql <path-to-database.db>
```

## Feature set

libSQL is a fork of SQLite, and we keep their original README [here](README-SQLite.md).

Aside from all the goodies already provided by SQLite, libSQL adds:

The comprehensive description can be found [here](doc/libsql_extensions.md)

