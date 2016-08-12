Location Aware Python
=====================

Encode & Decode Location Aware Names (Python port)

Location Aware Names, is a rethinking of how we give name to places, 
streets or locations by encoding information right into the letters 
that form the name

Project ported from https://github.com/roberdam/Locationawarenames 
(ruby to python) and also added python pip library and installation
Please see original project from roberdam since it includes a web API
and web service for encoding decoding with a map interface.

Installation
------------

	pip install location_aware

Calling examples
----------------

From term just execute to get the usage:
	
	location_aware


To convert from lat/lon to location aware name (process called encoding)
encoding of latitude: 50.0 & longitude: 6.0. And obtaining DEXA-DASA:

	location_aware -e 50 6

To decode from location aware name to latitude and longitude:

	location_aware -d RARI-NUCA

Library example
---------------

From python you just need to

	import location_aware

and and then just call encode and decode as usual

	location_aware.encode(65.7, -170.6)
	location_aware.decode('DEXA-DASA')

