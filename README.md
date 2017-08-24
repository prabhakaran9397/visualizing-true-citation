# Visualizing Citation Network

### Defining new index based on true children and visualizing its path.

There are 1 to 2092356 (inclusive) papers.

_citation.txt_ contains directed graph input where _child_ has cited its _parent_.

`parent child1,child2,child3,...`

Missing numbers in _citation.txt_ indicates that those parents does not have any children.

 
##### Cleansed Dataset
```
bash> cd dataset
bash> xz -vd citation.txt.xz
bash> xz -vd AMiner-Paper.sql.xz
bash> mysql -u username -p
mysql> create database citations;
mysql> exit;
bash> mysql -u username -p citations < AMiner-Paper.sql
```

##### Original Dataset
https://aminer.org/aminearnetwork