CONTENTS OF THIS FILE
---------------------

 * summary
 * configuration

SUMMARY
-------

This module is for adding support for entities (person, place, event,
organization) to Islandora.

CONFIGURATION
-------------

The Solr field for searching entities and the entity collection are
configurable at admin/islandora/entities.


Installation
------------

The MADS_to_solr.xslt from the data directory should be put in the
islandora_transforms directory, usually found in
$CATALINA_HOME/webapps/fedoragsearch/WEB-INF/classes/fgsconfigFinal/index/FgsIndex$ cd islandora_transforms

and it should be referenced in foxmlToSolr.xslt, if using a standard Islandora setup.
<xsl:include href="/usr/local/fedora/tomcat/webapps/fedoragsearch/WEB-INF/classes/fgsconfigFinal/index/FgsIndex/islandora_transforms/MADS_to_solr.xslt"/>