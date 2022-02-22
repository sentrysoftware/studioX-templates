CQL Queries Using a Command Line Monitor
====================================================
This template shows how to send CQL (Cassandra Query Language) queries within Monitoring Studio X, leveraging the Command Line monitor. As of the current version, we do not have a CQL query monitor, as such this is the simplest method of querying a Cassandra Database.  

This query leverages the cqlsh command which is typically shipped with every Cassandra package, usually found in the /bin folder alongside the Cassandra executable. You can refer to the [CQLSH reference document](https://docs.datastax.com/en/dse/5.1/cql/cql/cql_reference/cqlsh_commands/cqlshCommandsTOC.html) for query or sytax concerns.


<strong>Command Line Monitor - CQL Query Using cqlsh</strong>

Command run on host:
```bat
cqlsh -u %{USERNAME} -p %{PASSWORD} "SELECT * FROM tablename WHERE column='condition'"
```
In this monitor, we use the cqlsh command to call the cqlsh tool on the server. In this scenario, we used -u %{USERNAME} -p %{PASSWORD} in order to use the credentials specified in the host. Lastly, the string between quotation marks is the query we are sending to the Cassandra database.

Sample output:
```
John    Smith
Jane    Doe
Bob     Ross
```

From here, any content parsing monitors can be used to parse the output of the query as with any other monitors. (Dynamic Instances, Numeric Extractions, String Search, etc.)
