This repository is built for the open data connector and case studies based on KNIME Geospatial Extension. 

Backgroud :KNIME AG and Harvard’s Center for Geographic Analysis have launched a joint project to advance spatial 
data science. The project is part of the Spatiotemporal Thinking, Computing, and Applications (STC)
Center which is funded by the NSF to enable pre-competitive research in partnerships among industry, 
academia, and government. The two-year project “Developing Workbenches for Spatial Data Science (HVD-21-07)”
will explore methodologies to advance spatial data science research and teaching.
To open up spatial analytics to a more diverse group of users, the partners will develop freely accessible 
KNIME Analytics Platform extensions for spatial statistics, modeling, and visualization. KNIME’s visual,
no-code/low-code environment will enable multi-discipline users to more easily and efficiently collaborate, 
explore data, and surface insights. Further resources in the form of workbooks, workflow-based case studies,
and best-practice workflows will be developed to help users get started with replicable and reproducible spatial 
data science across scientific disciplines.

Workflow 01-US Census Data Connector.knwf

Citation:

Liu, Lingbo. "KNIME US Census Data Connector." Harvard Dataverse, 2022. https://doi.org/10.7910/DVN/LILUPH.

This workflow is the prototype of KNIME Python-based Geospatial Extension, which contains three nodes in Open Datasets Category.
User can easily get US TIGER/Line Data ( Base map of Census Block, Block Group, Tract and County in 2010 and 2020) ,
US 2020 Census data( Population) and American Community Survey (ACS) 5-years data.
The ACS-5 helps local officials, community leaders, and businesses understand the changes taking place in their communities. It is the premier source for detailed population and housing information about our nation.

Requirements

US Census API key :https://api.census.gov/data/key_signup.html 

KNIME Extension : KNIME Python Integration 

Python Package : geopandas, requests, matplotlib





