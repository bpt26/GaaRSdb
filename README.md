## Genomic Aminoacyl tRNA Synthetase database

This repository will eventually contain as much information as I can gather on aminoacyl tRNA synthetases, in the form of SQL queries. I am learning SQL by developing this database and am balancing several other projects, so progress may be slow. However, the end goal is to produce a fully functional database in which users can find sequences for aaRSs by tRNA isotype and species, as well as obtain orthologs of genes of interest for species where available.

Currently, there are all orthologs of human synthetases and related genes found using OrthoDB 10.

Example starter query to examine the data after initializing database:
```
use GaaRSdb ;
SELECT * FROM genes JOIN species ON genes.species_id = species.species_id JOIN og_oids ON genes.og_id = og_oids.og_id ;
```
