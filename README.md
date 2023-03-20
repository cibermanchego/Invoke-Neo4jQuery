# Invoke-Neo4jQuery
**This script is not mine (source: https://github.com/teal-technology-consulting/Invoke-Neo4jQuery)**
I only modified it to improve the CSV output plus compiled and adapted a lot of queries to be used out of the box, they are included in the file neo4j_queries.json.

It uses the Neo4j console directly instead of the Bloodhound interface and downloads the output in CSV format for later use.
It creates a new CSV file per query with the file name taken from the title in the JSON file.
Looking at the neo4j_queries.json file it's easy to see how to add new queries or remove the ones not needed.

The idea is to speed up the process of extracting interesting information from the Bloodhound database and have an easier format to work with.
Feel free to expand upon the quries already present in the neo4j_queries.json file.



How to run: 
```
Invoke-neo4jQuery "http://localhost:7474/db/bloodhound/tx/commit" neo4j_queries.json neo4j <NEO4J_PASSWORD> "c:\users\consultant\bloodhound\output"
```
More help inside the script.
