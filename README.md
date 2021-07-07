# Test DBCP with CockroachDB


### Code sample based on:
https://git-wip-us.apache.org/repos/asf?p=commons-dbcp.git;a=blob;f=doc/PoolingDataSourceExample.java;h=2a12c74898930b9623223db1597b8a8052a6f1df;hb=HEAD

### Run by passing the following arguments:
```
jdbc:postgresql://localhost:26257/defaultdb?ApplicationName=TestDBCP&ssl=true&sslcert=%2FUsers%2Fjimhatcher%2Flocal_certs%2Fclient.root.crt.der&sslkey=%2FUsers%2Fjimhatcher%2Flocal_certs%2Fclient.root.key.der&sslmode=verify-full&sslrootcert=%2FUsers%2Fjimhatcher%2Flocal_certs%2Fca.crt.der&user=root
"SELECT 1"
```
Notice that I'm passing the username as `&user=root` rather than `root@localhost:26257`; the latter syntax doesn't seem to work.