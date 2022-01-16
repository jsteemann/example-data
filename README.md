# Example data

This repository contains some made-up example data for test purposes.

The data can be imported into ArangoDB as follows:

1. start ArangoDB
2. download the file `dump.tar.gz` from this repository
3. extract `dump.tar.gz` somewhere in the local filesystem
4. run the following `arangorestore` command
```
arangorestore \
  <path to extract dump directory>  \
  --server.endpoint <endpoint>      \
  --server.username <username>      \
  --server.password <password>
```

Example:
```
arangorestore \
  /home/test/Downloads/dump>              \
  --server.endpoint tcp://127.0.0.1:8529  \
  --server.username root                  \
  --server.password ""
```
