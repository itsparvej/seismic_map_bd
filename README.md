"Mapping Bangladesh's Seismic Risks: 2001-2025 Earthquake Patterns Revealed" 
Using USGS earthquake data, I created a seismic risk map of Bangladesh, classifying zones from very low to very high risk. This helps visualize earthquake vulnerability for disaster preparedness and urban planning. A critical tool for policymakers, researchers, and communities! 
What It Shows: 
•	Data Span: Earthquake occurrences from 2001–2025 (magnitude, location). 
•	Risk Zones: 5-tier classification (very low to very high ) based on interpolated seismic activity. 

How to Make One for Yourself: 
1.	Data Collection: 
•	Download earthquake data (2001–2025) from USGS Earthquake Catalog . 
•	For download Bangladesh data, use Geographic region as custom and give the North, South, East, West location in the box.
•	Then download the data in csv format.

 
2.	Shapefile Prep: 
•	Get Bangladesh’s administrative boundary shapefile from GADM or DIVA-GIS or Hum data website. 
•	Then add the csv to ArcGIS and show it as xy table to point, select the magnitude field as Z field and longitude as x, latitude as x.
•	Then export this feature as shapefile.
•	Then clip the earthquake shapefile based on BD administrative boundary.
 
3.	Interpolation in ArcGIS Pro: 
•	Use Kernel Density or IDW tools to map seismic intensity. 
•	For IDW spatial analyst tool, select the earthquake shapefile as input point featur , select magnitude field as Z field value, give a output name and location and in Environments tab select coordinate system as wgs1984, select the Extent and Mask in Raster Analysis as bd shapefile.
 
4.	Risk Classification: 
•	Reclassify the interpolated raster into 5 zones using Equal Interval or Natural Breaks from the symbology pan of the IDW.
•	Then change the color as you like 
5.	Design & Export: 
•	Add legends, scale bars, and labels. Use color ramps (e.g., green → red) for clarity. 
•	Export as PDF/high-res image for sharing. 
Quotes: 
•	"Earthquakes don’t kill people—unpreparedness does. Let’s turn data into action." 
•	"Mapping risks today ensures safer cities tomorrow." 
Need Help? 
If you’re interested in replicating this project or need guidance for your region, feel free to reach out! I’m happy to share workflows, data sources, or troubleshoot GIS challenges. Let’s collaborate to build resilient communities. 🌍✨ 
Email: official.parvej.hossain@gmail.com
