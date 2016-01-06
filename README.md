The ittc tile services workflow is used to create the following **four** files
	*ittc_services_unflattened.geojson*
		This is used for the ITTC Services webmap.
	*ittc_services_flattened.geojson*
	*ittc_services_flattened.shp*
	*ittc_services_flattened.kml*
		These three files will be available for download and dissemination.

To obtain the four files you must use the following four files
	*getcapabilities_1.3.0.xml*
		Found on the HIU geoserver, this file can be downloaded via [this link](http://54.224.188.220:8080/geoserver/nextview/wms?service=WMS&version=1.1.0&request=GetCapabilities)
	
	*tilecache.cfg*
		Used to update tilecache.tsv this is found on the AWS server and nees a GIS analyst (read: Tom) to SSh into the server and retreive
		
	*tilecache_YYYMMDD.tsv*
		manually updated .tsv file that indicate the service, country, tasking manager number, and if it is a "valid" or "excluded" service.
		
	*geojsons_to_add.tsv*
		running list that is manually updated with services missing from the server
