Solr Extension for OpenCart Configuration Steps

index.php>>>>>>>>>>
//SOLR
$solrSearch=new SolSearch(SOLR\_HOSTNAME,SOLR\_PORT,SOLR\_INDEXPATH);
$registry->set('solrSearch', $solrSearch);


config.php>>>>>>>>>>>>>>>>>>>>>>>
/**START - SOLR CONNECTION SETTINGS**/
define('SOLR\_HOSTNAME', 'localhost');
define('SOLR\_PORT', '8983');
define('SOLR\_INDEXPATH', '/solr');
/**END - SOLR CONNECTION SETTINGS**/


inside library folder
>>>>>>>>>>>>>>>>>>>>>.
solr folder contains > solrsearch.php & phpSolrClient folder

system folder>>>
startup.php
require\_once(DIR\_SYSTEM . 'library/solr/solrsearch.php');//for solr search component