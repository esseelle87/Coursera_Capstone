This repository consists of:

6 codes notebooks:
	- ScrapingImmoscout24ch_FA.ipynb,
	- Scraping_foursquare_cat_FA.ipynb,
	- Geneva_POI_FA.ipynb,
	- Geneva_properties_FA.ipynb,
	- Cluster_geneva_properties_FA.ipynb.
	- Week5_assignment.ipynb: main report notebook:

	
6 files storing data scraped and analysed in the course of this project:
	- dic_all_cat.json,
	- GenevaRents_FA.json,
	- db_geneva_app_FA.json, 
	- geneva_allapp.csv,
	- README_CourseraCapstone.txt: this file,
	- Slideshow_capstone_project.pdf : presentation for this project.

6 folders:
	- "geneva_POI" where several cvs for running "Geneva_POI_FA.ipynb" are strored.
	- "venues_per_app", where several cvs files containing the nearby venues for each property are stored
	- "Images_from_ScrapingImmoscout24ch_FA.ipynb", with images for the final report.
	- "Images_from_GenevaLocations_FA", with images for the final report
	- "figures_ai", with images for the final report
	- "Images_from_ScrapingImmoscout24ch_FA.ipynb" , with images for the final report




The purpose of each notebook is briefly explained in the top markdowns.
The notebooks should be run as follow:

1)	Run "Scraping_foursquare_cat_FA.ipynb" and "Geneva_POI_FA.ipynb" in no particular order.
	The first one is used to create "dic_all_cat.json" to be used later.
	The second notebook has some code set as markdown. This code has been run once to create 
	"GenevaPOI.json". These part can be set again to 'code' again in case we would like to query 
	foursquare again. The notebook can be used as it is, and it will load data previously stored
	in the folder "geneva_POI". Here, each .csv file corresponds to the venues belonging to a
	 certain category in Geneva.
	
2)	Run "ScrapingImmoscout24ch_FA.ipynb".
	The lines used  for querying foursquare here are set as markdown. These lines have 
	been run once and the data has been stored in "GenevaRents_FA.json" .
	By default we could run the code as it is and load back the data from there
	(this is to allow the reviewer to use up his own foursquare calls.)

	The final output will be "db_geneva_app_FA.json" to be used later on.

3)	Run "Geneva_properties_FA.ipynb".
	This will create the file "geneva_allapp.csv", to be used later on.
	
4) Finally, run "Cluster_geneva_properties_FA.ipynb" for finalising the analysis.