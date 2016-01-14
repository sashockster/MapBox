# SchoolDangers-MapBox
==============================================
This repository is used to impliment MapBox visualizations for School Dangers Org's public website.

School Dangers Baselayers
----------------------------------------------
School Dangers baselayers (custom styled map backgrounds aka tiles) will be listed here in the future.

School Dangers Marker Data
----------------------------------------------
Map marker data is stored in /beta/data or /live/data as geoJSON files.


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
