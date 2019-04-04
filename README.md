# DEMNA-occurrences

Data publication DEMNA

## "MI" FILES ;

Are linked to first step for the publication of the 'AQUABIO' database. This database will be published in its integrality so exotic species will not be included into 'Exotic Animals in Wallonia' publication. MI is one of the 3 collections of the database that will have it's own GBIF publication (with fishes and macrophytes, after validation of the procedure the 2 others will follow : same steps for much much cleaner collections). 

Target publication = end of April 2019.

## "Fauna_Taxo" ;

It undertakes all animal taxa presents over all DEMNA's exploitable databases (Natagora, AQUABIO, and other databases not to include are already removed). Should only concern animals & shrooms. 
* Tax = raw encoding (might include some surprises)
* Taxprio= name for usage (unify synonyms or misspelings together). It should follow the same syntax rules for all species names but it is not always the case...
* Taxo_id should be attributed to each distinct taxprio. But the count do not match with the count of distinct taxprio...

 **TIP** : previous to do a taxa names comparison (eg. with unified checklist), I remove all ('sp.','spp.'sspp.','group', 'S.L', dobles spaces, etc.) from the columns tax & taxprio  to better fit a (genus||specificEpithet||InfraspecificEpithet) synthax. Also removing spaces at the start and at the end. There are many subtilities to identify accross DEMNA's taxa names that can alter the SQL string comparison...

Find and mark all exotic species among this list would be a very great input. Automated matching with SQL will match many, but the real problem are the one that do not match : is it really a native species? is it a synonym of a exotic specie? An invalid entry?




## "DEMNA excotics" ;

List of exotic species (internal to DEMNA : not complete enough). It should includes animals only. The full version is added in a second file, just in case.
* 'Prioritaire' refers to species included in the Union concern list.


## 'format eel'
Describes the structure under which we aggregate our differents databases to have a 'zoological fusion'.


### 'Taxons_trias'
* Imported from Trias Unified checklist.
* 'CanonicalName' = reformated to better match with the syntaxic rules for writting taxa names at DEMNA (genus||specificEpithet||InfraspecificEpithet) and so to subselect these taxa for publication.  


