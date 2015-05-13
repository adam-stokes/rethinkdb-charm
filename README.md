# Usage

    juju deploy rethinkdb

## Scale

    juju deploy rethinkdb-slave
    juju add-relation rethinkdb:rethinkdb-master rethinkdb-slave:rethinkdb-master
    juju add-unit rethinkdb-slave

## Administer

Get public IP for rethinkdb-master and connect with web browser:

http://10.0.3.86:8080

You can verify that the RethinkDB cluster is up and all servers are connected. Create
a few tables and after a few minutes the replicas will be available throughout
the cluster.

# Contact

[GitHub](https://github.com/battlemidget/rethinkdb-charm)
