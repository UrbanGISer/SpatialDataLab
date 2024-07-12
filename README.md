# SpatialDataLab- Spatiotemporal Innovation Workshop  2024

This Repository is for Spatiotemporal Innovation Workshop Held by Spatial Data Lab , Center for Geographic Analysis, Harvard Univeristy

More Detail :[Spatiotemporal Innovation Summer Workshop 2024](https://sdl.gis.harvard.edu/event/summer-workshop-spatiotemporal-innovation-2024)

Harvard DataVerse : [https://dataverse.harvard.edu/dataverse/sdl_dataverse](https://dataverse.harvard.edu/dataverse/sdl_dataverse)

KNIME Geospatial Extension : [https://github.com/spatial-data-lab/knime-geospatial-extension](https://github.com/spatial-data-lab/knime-geospatial-extension)

The workshop mainly use KNIME Analytic Platform and its Python Extension.

## Step 1: KNIME Installation

- **Go to the KNIME website （choose suitable version of Operation System）**

  [https://www.knime.com/downloads/download-knime](https://www.knime.com/downloads)

  Note:as the updating of KNIME is frequent, self-extrating archive is highly recommended for Windows**

- **Extract to a folder, double click KNIME.exe to start KNIME**

- **To get the best performance of KNIME, open knime.ini with Notepad(Windows)**

  revise -Xmx2048m  as -Xmx8g  ( 8 Giga Byte, or half for your computer memory)

- **Choose a directory as workspace（e.g. E:\KNIMEworkspace）,While starting KNIME**

    user can execute multiple KNIME APP simultaneously (same or different versions), but each KNIME Analysis Platform must use a unique directory as workspace;
    
    While run only one KNIME APP at a time, different versions of KNIME software can use the same workspace directory.
  

## Step 2:  Python Installation（Anaconda）

- **Go to Anaconda website and download**

  https://www.anaconda.com/ 

  Double click the installation file to run Anaconda

- **Star Anaconda Prompt or Anaconda，build a new Conda enviroment  of Python 3.9 for KNIME**

  conda create -n geoai python=3.9 knime-extension knime-python-base  -c conda-forge -c knime


- **Python packages**
    
    2-2-GeoAI
    pip install XGeoML mgwr geoshapley matplotlib  pygam 

    3-1-Network Community
    pip install  fiona python-igraph leidenalg pygeoda
    pip install torch torch_geometric
    refer to: https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html
  
    3-2-Remote Sensing
    pip install  rasterio folium mapclassify
    pip install earthengine-api geemap


##  Step 3: KNIME Extension 
- **Install Python and R extension in KNIME**

  open KNIME > File > Install KNIME extension , in the dialog
    
  input "Python" in the box of  type filter text bar  > check KNIME Python Integration > input "R Statistics" in the box of  type filter text bar  > check KNIME Interactive R Statistics Integration > next >... > Restart KNIME

- **Commomly used Extensions**
- 
    Geospatial Analytics Extension for KNIME
  
    KNIME H2O Machine Learning Integration
  
    KNIME XGBoost Integration
  
    KNIME Al Assistant (Labs)
  
    KNIME Al Extension
  
    KNlME Deep Learning - Keras Integration
  
    KNIME H20 Machine Learning Integration
  
    KNlME Interactive R Statistics Integration
  
    KNlME Machine Learning Interpretability Extension
  
    *KNIME Nodes for Scikit-Learn (sklearn) Algorithm
  
    *KNIME Parallel Chunk Loop Nodes
  
    *KNIME Statistics Nodes (Labs)
  
    *KNIME Web Interaction (Labs)
  
    KNIME XGBoost Integration
  
    *Redfield NLP Nodes
  
    KNIME Column Expressions (Labs)
  
    KNIME Plotly
  
    KNIME Data Generation
  
    KNlME Textprocessing Chinese Language Pack
  
##  Step 4: Default Python Environment for Deep learning



## R and RStudio Desktop 
- **Go to CRAN website to download R package**

  https://cran.r-project.org/
  
  choose suitable version of Operation System
  
  e.g. R 4.2.1 for Windows :  https://cran.r-project.org/bin/windows/base/
  
  Recommend : Download R for Windows > Install R for the first time > Previous releases>  R 4.1.3 (March, 2022)

- **RStudio Installation （RStudio is not necessary）**

  Go to RStudio website 
  
  https://www.rstudio.com/products/rstudio/download/
  
  https://download1.rstudio.org/desktop/windows/RStudio-2022.07.1-554.exe
  
  Double click to install it.
  
- **Install Rserve package**

  Rserve is the basic pacakge to run R extension 
  
  for KNIME R 4.2.x might need to install its source data directly.https://www.rforge.net/Rserve/files/
  
  the best way to install Rserve without installing RStudio
  
  **install.packages('Rserve', dependencies = TRUE)**



##  KNIME Extension and Configuration

- **Install Python and R extension in KNIME**

  open KNIME > File > Install KNIME extension , in the dialog
    
  input "Python" in the box of  type filter text bar  > check KNIME Python Integration > input "R Statistics" in the box of  type filter text bar  > check KNIME Interactive R Statistics Integration > next >... > Restart KNIME
 
 - **Configuring R and Python enviroment in KNIME**
 
  open KNIME > File > Preference, in the dialog
  
  KNIME > Conda > click Browse... to choose the installed Anaconada directory, such as : D:\ProgramData\Anaconda3
  
  KNIME > Python > choose py37(or other environment) for Python3 (defult)
  
  KNIME >R >click Browse... to choose the installed R directory, such as C:\Program Files\R\R-4.2.1
  
  click Apply and Close.
 
 
