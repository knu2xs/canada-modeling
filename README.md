# canada-modeling

Modeling examples for Canadian demonstration. All the notebooks I showed are in the ./notebooks directory.

## References

### Top Level Resources
 
 - [ArcGIS Python API](https://developers.arcgis.com/python/)
 - Demographic Modeling Module [Github Repo](https://github.com/knu2xs/demographic-modeling-module) and [Docs](https://knu2xs.github.io/demographic-modeling-module/)
 - [GeoAI-Cookiecutter](https://github.com/esri/geoai-cookiecutter) - not discussed in the meeting, but what I used to build this whole project and just about every other project I work on...

### Topical References

- Geocoding
	- [ArcGIS.Geocoding module](https://developers.arcgis.com/python/api-reference/arcgis.geocoding.html)
	- [GeoAccessor.from_df method](https://developers.arcgis.com/python/api-reference/arcgis.features.toc.html#arcgis.features.GeoAccessor.from_df)
- GeoEnrichment
	- [ArcGIS.Geoenrichment module](https://developers.arcgis.com/python/api-reference/arcgis.geoenrichment.html)
	- [Demographic Modeling's enrich accessor method](https://knu2xs.github.io/demographic-modeling-module/dm.html#dm.DemographicModeling.enrich)
    - [Apportionent Methodlogy Explained](https://developers.arcgis.com/rest/geoenrichment/api-reference/data-apportionment.htm) (applies to US _and_ Canada)
- Transportation Network Analysis
	- [Origin-Destination - ODCostMatrixLayer](https://developers.arcgis.com/python/api-reference/arcgis.network.toc.html#odcostmatrixlayer)
	- [Isochromes - ServiceAreaLayer](https://developers.arcgis.com/python/api-reference/arcgis.network.toc.html#servicearealayer)
- Places of Interest (Businesses)
	- [Demographic Modeling's Business object](https://knu2xs.github.io/demographic-modeling-module/dm.html#dm.Business)
- ArcGIS Python Toolbox
    - [What is a Python Toolbox](https://pro.arcgis.com/en/pro-app/latest/arcpy/geoprocessing_and_python/a-quick-tour-of-python-toolboxes.htm)
    - [Creating a New Python Toolbox](https://pro.arcgis.com/en/pro-app/latest/arcpy/geoprocessing_and_python/creating-a-new-python-toolbox.htm) - start of the detailed docs on this
    
### Published Vancouver Examples

- Vancouver Web Map
    - [Item in ArcGIS Online](https://arcgis.com/home/item.html?id=0094d39e499444f8b5d65f504f5235cf)
    - [Direct Link to Interactive Web Map](https://arcgis.com/apps/mapviewer/index.html?webmap=0094d39e499444f8b5d65f504f5235cf)
- Vancouver Web Application
    - [Item in ArcGIS Online](https://arcgis.com/home/item.html?id=0d4047b980a64026a6fbb7510565497a)
    - [Direct Link to Interactive Application](https://arcgis.com/apps/View/index.html?appid=0d4047b980a64026a6fbb7510565497a)

## Project Organization
------------
```
    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data`
    ├── make.bat           <- Windows batch file with commands like `make data`
    ├── setup.py           <- Setup script for the library (canada_modeling)
    ├── .env               <- Any environment variables here - created as part of project creation, 
    │                         but NOT syncronized with git repo for project.                
    ├── README.md          <- The top-level README for developers using this project.
    ├── arcgis             <- Root location for ArcGIS Pro project created as part of
    │   │                     data science project creation.
    │   ├── canada-modeling.aprx <- ArcGIS Pro project.    
    │   └── canada-modeling.tbx  <- ArcGIS Pro toolbox associated with the project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    ├── notebooks          <- Jupyter notebooks. Naming convention is a 2 digits (for ordering),
    │   │                     descriptive name. e.g.: 01_exploratory_analysis.ipynb
    │   └── notebook_template.ipynb
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    ├── environment.yml    <- Requirements file for reproducing the analysis execution environment.
    │                         This includes far fewer dependencies and does not include arcpy.
    ├── environment_dev.yml<- Requirements file for reproducing the analysis deveopment environment.
    │                         This includes arcpy and everything needed to generate Sphinx docs.
    └── src                <- Source code for use in this project - all scripts, modules and code.
        └── canada_modeling <- Library containing the bulk of code used in this 
                                                  project. 
```

<p><small>Project based on the <a target="_blank" href="https://github.com/knu2xs/cookiecutter-geoai">cookiecutter GeoAI project template</a>. This template, in turn, is simply an extension and light modification of the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
