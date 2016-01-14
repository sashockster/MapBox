# SchoolDangers-MapBox      VERSION:*BETA*
==============================================
This repository is intended to help developers visualize School Dangers Org's school incident and school location data using the MapBox.com service.  This work will also be used by School Dangers Org's public website.

The current version is *BETA*, meaning we have a framework, but it is not *copy-and-paste* ready for primetime.  

## School Dangers Baselayers
----------------------------------------------
School Dangers baselayers (custom styled map backgrounds aka tiles) will be listed here in the future.  For now we are using *mapbox.streets*, but plan to release a less cluttered background map to help viewers focus on schools and school incidents.

## School Dangers Incident Marker Data
----------------------------------------------
*BETA* map marker data is stored in /beta/data as geoJSON files.

Several *BETA* geoJSON files are provided as examples of data structure and size for incidents and school locations.  These files are not intended for production. For example, our geoJSON file of 100,000+ schools is 42MB and early testing has shown people fall asleep or speak crudely to their computers as the file downloads and javascript draws the markers. 

The primary geoJSON file is incidents.geojson.  
As we get closer to version 1.0, it is our intention that the live version of the file be published from our online database nightly and accessed using an api key so we can build some awesome statistics.


### GeoJSON structure for School Dangers Map Features (Incidents): ###
----------
	Incident Markers
		var geojson = [
		  {
		    "type": "Feature",
		    "geometry": {
		      "type": "Point",
		      "coordinates": [-77.03238901390978,38.913188059745586]
		    },
		    "properties": {
		      "title": "Name of School Incident Occurred",
		      "description": "Summary of the incident",
		      "marker-color": "#fc4353",
		      "marker-size": "small",
		      "marker-symbol": "marker",
		      "incident-date": "5\/18\/1978 0:00", 
		      "Year": 1978, 
		      "incident-type": "Shooting", 
		      "casualties": 1, 
		      "injuries": 0,
		      “city”: “City”,
		      “state”: “ST”,
		      “facility-type”: “K-12”,
		      "facility-subtype": "Secondary", 
		      "perpetrator": "persons name",
		      "perpetrator-fate": "Arrested",
		      "foiled": "Yes", 
		      "included-in-2002-report": “true/false”
		    }
		  }
		];
