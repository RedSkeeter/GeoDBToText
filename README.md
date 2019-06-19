# GeoDBToText
![GeoDBToText icon](GeoDBToText.png "Geodatabase to text files")

One goal of long term ecosystem monitoring programs is to preserve data in non-proprietary human and machine readable ASCII text file formats. Additionally, the U.S. government requires non-sensitive data to be publicly available in human and machine readable formats (see https://project-open-data.cio.gov/).

ESRI geodatabases are highly functional for day to day use but are highly likely to be unsupported/unreadable decades in the future and do not meet open data requirements. The GeoDBToText tool prevents data loss by exporting each feature class in an ESRI personal geodatabase (.mdb) to human and machine text (pipe separated values/WKT, ESRI JSON) file formats. Should the original geodatabase be unusable the text files generated by this tool should still be recoverable. The National Park Service Arctic and Central Alaska Inventory and Monitoring Networks archive proprietary geospatial datasets in tandem with human and machine readable text file formats.

Written by Scott D. Miller, Data manager, National Park Service Arctic Network Inventory and Monitoring Program, Fairbanks, AK.
https://www.nps.gov/im/arcn/index.htm
2019-06-19
Tested against ArcGIS 10.6.1

# How to use
1. Download the files from this GitHub repository.
2. Navigate to the GeoDBToText.tbx and open it.
3. Right click the 'Geodatabase to text files' Python script tool.
4. Click the Source tab
5. Ensure the 'Script file' text box contains the correct path to GeoDBToText.py script.
6. Execute the script by double clicking and follow the prompts

The text files will be named according to the feature class they represent and will be exported into the same directory as the source geodatabase. Existing files will be overwritten without confirm.
