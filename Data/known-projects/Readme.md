Process for creating data in this folder:

zcat /da?_data/basemaps/gz/A2PFullV?.s | cut -d\; -f2 | grep -e '^apache_' | sort -u > "apache-projects.txt"

This is done for each of the following Foundations and their associated grep patterns:

* ASF: '^apache_'
* Eclipse: '^eclipse_'
* Cloud foundry: '^cloundfoundry_'
* Kuali: '^kuali_'
* Osgeo: '^OSGeo_'
* Oregon State University Open Source Lab Alliance: '^osuosl_'
	
