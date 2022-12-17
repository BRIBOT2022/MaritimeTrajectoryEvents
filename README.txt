-----------------------------------------------------------------------------------------------------
-- Object : netWorkData
-- File name : routePolygon
-- Source : Automatic Identification System
-- Dataset version : v1 (31/05/2022)
-- SRID : WGS84 
-- Coverage : East Longitude between 117°35′ and 121°10′ and North Latitude between 37°07′ and 41°0′
-- Volume : 118 topology files 
-- Period : 3 months (2018-01-01 00:00:00 UTC to 2018-03-31 23:59:59 UTC)
-- Licence : CC-BY-NC-SA-4.0
-- Description : Each file saves marked route segment polygons
-----------------------------------------------------------------------------------------------------
Attribute		Data type		Description
-----------------------------------------------------------------------------------------------------
*  lon 		double precision  	Longitude (georeference: WGS 1984)
*  lat 		double precision 	Latitude  (georeference: WGS 1984)
-----------------------------------------------------------------------------------------------------
-- Object : netWorkData
-- File name : edge
-- Source : Automatic Identification System
-- Dataset version : v1 (31/05/2022)
-- SRID : WGS84 
-- Coverage : East Longitude between 117°35′ and 121°10′ and North Latitude between 37°07′ and 41°0′
-- Volume : 120 pieces of data
-- Period : 3 months (2018-01-01 00:00:00 UTC to 2018-03-31 23:59:59 UTC)
-- Licence : CC-BY-NC-SA-4.0
-- Description : The file saves the edges in the channel network. There are 3 fields. The first field is the road segment id, and the second and third fields are the start/end node id of the road segment.
-----------------------------------------------------------------------------------------------------
Attribute		Data type		Description
-----------------------------------------------------------------------------------------------------
*  segment id  	integer    	segment id  
*  start node	integer     The start node of the current road segment
*  end node	integer     The end node of the current road segment
-----------------------------------------------------------------------------------------------------
-- Object : netWorkData
-- File name : node
-- Source : Automatic Identification System
-- Dataset version : v1 (31/05/2022)
-- SRID : WGS84 
-- Coverage : East Longitude between 117°35′ and 121°10′ and North Latitude between 37°07′ and 41°0′
-- Volume : 102 pieces of data
-- Period : 3 months (2018-01-01 00:00:00 UTC to 2018-03-31 23:59:59 UTC)
-- Licence : CC-BY-NC-SA-4.0
-- Description : The file saves the nodes in the channel network and has 4 fields, namely node id, node longitude, node latitude, and node type.
-----------------------------------------------------------------------------------------------------
Attribute		Data type		Description
-----------------------------------------------------------------------------------------------------
*  node id  	integer    		node id  
*  lon 		double precision  	Longitude (georeference: WGS 1984)
*  lat 		double precision 	Latitude  (georeference: WGS 1984)
*  node type	integer     	node type
-----------------------------------------------------------------------------------------------------
-- Object : netWorkData
-- File name : topology
-- Source : Automatic Identification System
-- Dataset version : v1 (31/05/2022)
-- SRID : WGS84 
-- Coverage : East Longitude between 117°35′ and 121°10′ and North Latitude between 37°07′ and 41°0′
-- Volume : 102 pieces of data
-- Period : 3 months (2018-01-01 00:00:00 UTC to 2018-03-31 23:59:59 UTC)
-- Licence : CC-BY-NC-SA-4.0
-- Description : The file saves the channel network topology relationship. The first field of each line is the current node's id, and the following fields are the nodes' ids adjacent to it.
-----------------------------------------------------------------------------------------------------
Attribute		Data type		Description
-----------------------------------------------------------------------------------------------------
*  node id  		integer    	node id  
*  neighbor node id1	integer     neighbor node id
*  neighbor node id2	integer     neighbor node id
*  neighbor node id3	integer     neighbor node id
*  …………
-----------------------------------------------------------------------------------------------------
-- Object : BohaiData-2018010203-preprocessed
-- File name : bohai-segment1-inlane
-- Source : Automatic Identification System
-- Dataset version : v1 (31/05/2022)
-- SRID : WGS84 
-- Coverage : East Longitude between 117°35′ and 121°10′ and North Latitude between 37°07′ and 41°0′
-- Volume : 1446 data files
-- Period : 3 months (2018-01-01 00:00:00 UTC to 2018-03-31 23:59:59 UTC)
-- Licence : CC-BY-NC-SA-4.0
-- Description : This data is the AIS data of Bohai after segmentation, sampling, denoising, interpolation and channel network matching. Each file saves a trip record and contains 3 fields, namely timestamp, longitude and latitude.
-----------------------------------------------------------------------------------------------------
Attribute		Data type		Description
-----------------------------------------------------------------------------------------------------
*  timestamp	integer    		timestamp		
*  lon 		double precision  	Longitude (georeference: WGS 1984)
*  lat 		double precision 	Latitude  (georeference: WGS 1984)
-----------------------------------------------------------------------------------------------------
-- Object : BohaiData-2018010203-preprocessed
-- File name : bohai-segment2-inlane
-- Source : Automatic Identification System
-- Dataset version : v1 (31/05/2022)
-- SRID : WGS84 
-- Coverage : East Longitude between 117°35′ and 121°10′ and North Latitude between 37°07′ and 41°0′
-- Volume : 2125 data files
-- Period : 3 months (2018-01-01 00:00:00 UTC to 2018-03-31 23:59:59 UTC)
-- Licence : CC-BY-NC-SA-4.0
-- Description : This data is the AIS data of Bohai after segmentation, sampling, denoising, interpolation and channel network matching. Each file saves a trip record and contains 3 fields, namely timestamp, longitude and latitude.
-----------------------------------------------------------------------------------------------------
Attribute		Data type		Description
-----------------------------------------------------------------------------------------------------
*  timestamp	integer    		timestamp		
*  lon 		double precision  	Longitude (georeference: WGS 1984)
*  lat 		double precision 	Latitude  (georeference: WGS 1984)
-----------------------------------------------------------------------------------------------------
-- Object : Bohai--serialize
-- File name : bohai-segment1-inlane-serialize-type
-- Source : Automatic Identification System
-- Dataset version : v1 (31/05/2022)
-- SRID : WGS84 
-- Coverage : East Longitude between 117°35′ and 121°10′ and North Latitude between 37°07′ and 41°0′
-- Volume : 1349 data files
-- Period : 3 months (2018-01-01 00:00:00 UTC to 2018-03-31 23:59:59 UTC)
-- Licence : CC-BY-NC-SA-4.0
-- Description : The data is the serialized result of BohaiData-2018010203-preprocessed. Each file saves the serialized result of one trip and contains 6 fields, namely the id of the passed road, timestamp, longitude, latitude, sailing direction angle, and ship type.
-----------------------------------------------------------------------------------------------------
Attribute			Data type		Description
-----------------------------------------------------------------------------------------------------
*  segment id  		integer    		segment id  
*  timestamp		integer    		timestamp		
*  lon 			double precision  	Longitude (georeference: WGS 1984)
*  lat 			double precision 	Latitude  (georeference: WGS 1984)
*  sailing direction angle	double precision 	sailing direction angle
*  ship type		integer 		ship type（-1:others;0:fishing boat;1:cargo ship;2:cruise ship;3:passenger ship;4:Container Ship）
-----------------------------------------------------------------------------------------------------
-- Object : Bohai--serialize
-- File name : bohai-segment2-inlane-serialize-type
-- Source : Automatic Identification System
-- Dataset version : v1 (31/05/2022)
-- SRID : WGS84 
-- Coverage : East Longitude between 117°35′ and 121°10′ and North Latitude between 37°07′ and 41°0′
-- Volume : 1962 data files
-- Period : 3 months (2018-01-01 00:00:00 UTC to 2018-03-31 23:59:59 UTC)
-- Licence : CC-BY-NC-SA-4.0
-- Description : The data is the serialized result of BohaiData-2018010203-preprocessed. Each file saves the serialized result of one trip and contains 6 fields, namely the id of the passed road, timestamp, longitude, latitude, sailing direction angle, and ship type.
-----------------------------------------------------------------------------------------------------
Attribute			Data type		Description
-----------------------------------------------------------------------------------------------------
*  segment id  		integer    		segment id  
*  timestamp		integer    		timestamp		
*  lon 			double precision  	Longitude (georeference: WGS 1984)
*  lat 			double precision 	Latitude  (georeference: WGS 1984)
*  sailing direction angle	double precision 	sailing direction angle
*  ship type		integer 		ship type（-1:others;0:fishing boat;1:cargo ship;2:cruise ship;3:passenger ship;4:Container Ship）
-----------------------------------------------------------------------------------------------------

