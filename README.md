# Callisto Repository
List of useful datasets

## Callisto Generated Datasets

- [Mapillary Annotated](https://github.com/Agri-Hub/Mapillary_Annotation) <br/>
Crop type labels from the freely available Land Parcel Identification System (LPIS) of the Netherlands are matched with all available Mapillary street-level images for the year 2017. [[GitHub]](https://github.com/Agri-Hub/Callisto/tree/main/Mapillary) 

Relevant implementation applicable to this dataset: [Street2Sat](https://github.com/nasaharvest/street2sat_website/tree/ICML_paper_code), [DenseASPP](https://github.com/DeepMotionAIResearch/DenseASPP), [Crop Phenology](https://github.com/Momut1/flevoland)

- [Paddy Rice Maps South Korea (2017~2021)](https://github.com/Hyun-Woo-Jo/Paddy_Rice_Maps-South_Korea-2017_2021) <br />
 This dataset includes paddy rice maps in South Korea from 2017 to 2021 with 10m resolution. The paddy rice maps are a product of deep learning model predictions and DO NOT represent ground truth information. The predictions were made by analyzing time series Sentinel-1 images based on the deep learning architecture that integrates U-Net and RNNs layers desined by eGIS/RS lab, Korea University. The deep learning model has been trained on the farm map produced by the Korean Ministry of Agriculture, Food and Rural Affairs(MAFRA). The validation accuracy and Cohen's kappa value are 96.50%, 0.7857 each which were calculated from the 40% of the farm map. For more information please contact to the KU-eGIS/RS lab.
 
- [Paddy Rice Labeling Sites in South Korea (2018)](https://916e49e3-4865-4754-af5f-be19c7f09272.filesusr.com/archives/0832c0_ed10f249bbc146dbb34a07e4c6f11ab4.zip?dn=Label_VisuallyInterpreted.zip) <br />
  The paddy rice was visually interpreted at 30 sites in South Korea. The sites were selected at each province by a proportional stratified sampling method according to the paddy rice area statistics (Statistics Korea), so the dataset can be used for the validation on model generalization over the entire country. The paddy rice areas were visually interpreted by using Google Earth Pro and street view services (https://map.naver.com, https://map.kakao.com) and updated to the state of 2018.
  
## Existing Datasets

### Analysis Ready Sentinel Data

- [EarthNet2021 dataset](https://www.earthnet.tech/docs/ds-download/)
  - Training data for Earth surface prediction. The data consists of time series of Sentinel-2 products. More information can be found [here](https://www.earthnet.tech/docs/ds-specifications/) and [here](https://www.youtube.com/watch?v=sumLCeZ92Hk).
  [[Paper]](https://openaccess.thecvf.com/content/CVPR2021W/EarthVision/html/Requena-Mesa_EarthNet2021_A_Large-Scale_Dataset_and_Challenge_for_Earth_Surface_Forecasting_CVPRW_2021_paper.html) [[GitHub]](https://github.com/earthnet2021/earthnet-model-intercomparison-suite) 
  
- [BigEarthNet dataset](http://bigearth.net/#downloads)
  - BigEarthNet is a benchmark archive, consisting of 590,326 pairs of Sentinel-1 and Sentinel-2 image patches.
  - To construct BigEarthNet with Sentinel-2 image patches (called as BigEarthNet-S2 now, previously BigEarthNet), 125 Sentinel-2 tiles acquired between June 2017 and May 2018 over the 10 countries (Austria, Belgium, Finland, Ireland, Kosovo, Lithuania, Luxembourg, Portugal, Serbia, Switzerland) of Europe were initially selected. All the tiles were atmospherically corrected by the Sentinel-2 Level 2A product generation and formatting tool (sen2cor). Then, they were divided into 590,326 non-overlapping image patches. Each image patch was annotated by the multiple land-cover classes (i.e., multi-labels) that were provided from the CORINE Land Cover database of the year 2018 (CLC 2018). The labels in BigEarthNet belong to the initial release of the labels in 2018. 
  - To construct BigEarthNet with Sentinel-1 image patches (called as BigEarthNet-S1), 321 Sentinel-1 scenes acquired between June 2017 and May 2018 that jointly cover the area of all original 125 Sentinel-2 tiles with close temporal proximity were selected and processed. BigEarthNet-S1 consists of 590,326 preprocessed Sentinel-1 image patches - one for each Sentinel-2 patch. A more detailed explanation on the processing is given in its dataset description document.  <br />
  [[Paper (2019)]](http://bigearth.net/static/documents/BigEarthNet_IGARSS_2019.pdf) [[Paper (2021)]](https://arxiv.org/abs/2105.07921) [[Github]](https://git.tu-berlin.de/rsim)
 
- [So2Sat](https://mediatum.ub.tum.de/1483140)  <br />
  So2Sat LCZ42 consists of local climate zone (LCZ) labels of about half a million Sentinel-1 and Sentinel-2 image patches in 42 urban agglomerations (plus 10 additional smaller areas) across the globe. This dataset was labeled by 15 domain experts following a carefully designed labeling work flow and evaluation process over a period of six months. [[Paper]](https://ieeexplore.ieee.org/document/9014553) [[GitHub]](https://github.com/zhu-xlab/So2Sat-LCZ42)

- [EuroSAT dataset](https://github.com/phelber/EuroSAT) <br />
  27000 labeled and geo-referenced Sentinel 2 satellite image patches (i.e., 64  64 pixels). Although the classification scheme is made up of 10 different classes, including land covers having peculiar temporal patterns (i.e., annual crops, permanent crops), the dataset is based on single time images.  <br />
  [[Paper]](https://ieeexplore.ieee.org/document/8519248) [[GitHub]](https://github.com/phelber/EuroSAT)

- [Sen12MS](https://mediatum.ub.tum.de/1474000) <br />
  The SEN12MS dataset contains 180,662 patch triplets of corresponding Sentinel-1 dual-pol SAR data, Sentinel-2 multi-spectral images, and MODIS-derived land cover maps. The patches are distributed across the land masses of the Earth and spread over all four meteorological seasons. This is reflected by the dataset structure. All patches are provided in the form of 16-bit GeoTiffs containing the following specific information:
  - Sentinel-1 SAR: 2 channels corresponding to sigma nought backscatter values in dB scale for VV and VH polarization.
  - Sentinel-2 Multi-Spectral: 13 channels corresponding to the 13 spectral bands (B1, B2, B3, B4, B5, B6, B7, B8, B8a, B9, B10, B11, B12).
  - MODIS Land Cover: 4 channels corresponding to IGBP, LCCS Land Cover, LCCS Land Use, and LCCS Surface Hydrology layers. <br />
 [[Paper]](https://arxiv.org/pdf/1906.07789.pdf) [[GitHub]](https://github.com/schmitt-muc/SEN12MS)

- [SAT-4](https://www.kaggle.com/crawford/deepsat-sat4)<br />
  Originally, images were extracted from the National Agriculture Imagery Program (NAIP) dataset. The SAT-4 contains 500,000 RGB images. Each sample image is 28x28 pixels (1m spatial resolution) and consists of 4 bands - red, green, blue and near infrared. Each image is annotated with one of the four classes that represent four broad land covers which include barren land, trees, grassland and a class that consists of all land cover classes other than the above three. [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2820783.2820816)

- [SAT-6](https://www.kaggle.com/crawford/deepsat-sat6)<br />
  Originally, images were extracted from the National Agriculture Imagery Program (NAIP) dataset. The SAT-4 contains 405,000 RGB images. Each sample image is 28x28 pixels (1m spatial resolution) and consists of 4 bands - red, green, blue and near infrared. Each image is annotated with one of the six classes that represent six broad land covers which include barren land, trees, grassland, roads, buildings and water bodies. [[Paper]](https://dl.acm.org/doi/pdf/10.1145/2820783.2820816)
  
### Crop Classification Datasets

- [ZueriCrop](https://polybox.ethz.ch/index.php/s/uXfdr2AcXE3QNB6) <br />
  The ZueriCrop dataset contains ground truth labels of 116,000 field instances. Each field instance consists of a polygon representing the borders of the field, and its dominant crop label in 2019. The ground truth labels of all 48 crop classes are provided by the Swiss Federal Office for Agriculture (FOAG) and correspond to the primary crop grown per field during the year. The input data is a time series of 71 multi-spectral Sentinel-2 Level-2A bottom-of-atmosphere reflectance
images with a ground sampling distance (GSD) of 10 meters. All input images are atmospherically corrected using the Sen2Cor v2.8 software package. The dataset
is collected over a 50 km × 48 km area in the Swiss Cantons of Zurich and Thurgau between January 2019 and December 2019. The entire scene is subdivided into smaller patches of 24 px×24 px. Patches without any ground-truth information are discarded. In the remaining patches the fraction of pixels without reference label is ≈48%. Only those four spectral channels available at the highest, 10 m resolution (Red, Green, Blue, and Near-Infrared) are used. [[Paper]](https://arxiv.org/pdf/2102.08820.pdf) [[GitHub]](https://github.com/0zgur0/ms-convSTAR)

- [CV4A Kenya](https://mlhub.earth/10.34911/rdnt.dw605x)  <br />
  This dataset was produced as part of the Crop Type Detection competition at the Computer Vision for Agriculture (CV4A) Workshop at the ICLR 2020 conference. The ground reference data were collected by the PlantVillage team, and Radiant Earth Foundation curated the training dataset after inspecting and selecting more than 4,000 fields from the original ground reference data. The dataset has been split into training and test sets (3,286 in the train and 1,402 in the test).
The dataset is cataloged in four tiles. These tiles are smaller than the original Sentinel-2 tile that has been clipped and chipped to the geographical area that labels have been collected. Each tile has a) 13 multi-band observations throughout the growing season. Each observation includes 12 bands from Sentinel-2 L2A product, and a cloud probability layer. The twelve bands are [B01, B02, B03, B04, B05, B06, B07, B08, B8A, B09, B11, B12]. The cloud probability layer is a product of the Sentinel-2 atmospheric correction algorithm (Sen2Cor) and provides an estimated cloud probability (0-100%) per pixel. All of the bands are mapped to a common 10 m spatial resolution grid.; b) A raster layer indicating the crop ID for the fields in the training set; and c) A raster layer indicating field IDs for the fields (both training and test sets). Fields with a crop ID of 0 are the test fields. [[Paper]](https://arxiv.org/abs/2004.03023) [[GitHub]](https://github.com/RadiantMLHub/crop-type-detection-ICLR-2020)
  
- [TimeSen2Crop](https://drive.google.com/drive/folders/19YzUp0KhRnQN3IlU72vhJhCnzNJgFpsb) <br />
  A Million Labeled Samples Dataset of Sentinel 2 Image Time Series for Crop Type Classification [[Paper]](https://ieeexplore.ieee.org/abstract/document/9408357)
  
- [Sen4AgriNet](https://www.sen4agrinet.space.noa.gr/) <br />
  The Sen4AgriNet dataset is built using Sentinel-2 images from different timestamps include all spectral bands that have different spatial resolution.
  On top of the dataset, it has been developed a series of functions such as spatio-temporal aggregations, to transform the original dataset according to the different AI problems.
  - 5-year multitemporal Sentinel-2 patches 
  - Sentinel-1/2 data
  - The initial version of Sen4AgriNet consists of approximately 225,000. Corregistered with open LPIS data for regions in Spain and France with a total size of 10TB <br/>
  [[Paper]](https://ieeexplore.ieee.org/document/9553603) [[GitHub]](https://github.com/dimzog/S4A)


- [BreizhCrops](https://breizhcrops.org/)  <br />
  BreizhCrops is a novel benchmark dataset for the supervised classification of field crops from satellite time series. It contains
aggregated label data and Sentinel-2 top-of-atmosphere as well as bottom-of-atmosphere time series in the region of Brittany (Breizh
in local language), north-east France. [[Paper]](https://www.int-arch-photogramm-remote-sens-spatial-inf-sci.net/XLIII-B2-2020/1545/2020/isprs-archives-XLIII-B2-2020-1545-2020.pdf) [[GitHub]](https://github.com/dl4sits/breizhcrops) 

- Crop Type Mapping - Semantic Segmentation Datasets in [Ghana](http://registry.mlhub.earth/10.34911/rdnt.ry138p/) and [South Sudan](http://registry.mlhub.earth/10.34911/rdnt.v6kx6n/) <br />
  The datasets include time series of satellite imagery from Sentinel-1, Sentinel-2, and PlanetScope satellites throughout 2016 and 2017. For each tile/chip in the dataset, there are time series of imagery from each of the satellites, as well as a corresponding label that defines the crop type at each pixel. The label has only one value at each pixel location, and assumes that the crop type remains the same across the full time span of the satellite image time series. In many cases where ground truth was not available, pixels have no label and are set to a value of 0. For even more info, check the [[Paper]](https://openaccess.thecvf.com/content_CVPRW_2019/papers/cv4gc/Rustowicz_Semantic_Segmentation_of_Crop_Type_in_Africa_A_Novel_Dataset_CVPRW_2019_paper.pdf) and [[GitHub]](https://github.com/roserustowicz/crop-type-mapping) 
  
- [CaneSat dataset](https://ieee-dataport.org/documents/canesat) <br />
  CaneSat dataset contains sugarcane crop image samples and nonsugarcane samples. The image patches are generated from the Sentinel2 satellite images. [[Paper]](https://www.sciencedirect.com/science/article/pii/S1319157820304602)
  
- [Spot the Crop Challenge](https://mlhub.earth/10.34911/rdnt.j0co8q) <br />
  The dataset contains a time-series of satellite imagery and labels for crop type that have been collected through aerial and ground survey. Labels are derived from the survey conducted by the Western Cape Department of Agriculture, for the period of 04-01-2017 to 11-31-2017 and the area of Western Cape, South Africa. Satellite data including multispectral Sentinel-2 are then matched with corresponding labels. The S2 time-series is provided every 5 days. Sentinel-1 data include VV and VH backscatter with a time window of 12 days. The label chips contain the mapping of pixel to crop type label. The following pixel values correspond to the following crop types.
  - 0 - No Data
  - 1 - Lucerne/Medics
  - 2 - Planted pastures (perennial)
  - 3 - Fallow
  - 4 - Wine grapes
  - 5 - Weeds
  - 6 - Small grain grazing
  - 7 - Wheat
  - 8 - Canola
  - 9 - Rooibos
  
- [DENETHOR dataset](https://platform.ai4eo.eu/ai4food-security-germany) <br />
 DENETHOR: The DynamicEarthNET dataset for Harmonized, inter-Operabel, analysis-Ready, daily crop monitoring from space. Our dataset contains daily, analysis-ready Planet Fusion data together with Sentinel-1 radar and Sentinel-2 optical time-series for crop type classification in Northern Germany. The dataset includes: i) The Planet Fusion Monitoring product, which consists of clean (i.e. free from clouds and shadows), daily gap-filled, high resolution (3m), temporally consistent, radiometrically robust, harmonized and sensor agnostic surface reflectance time series, featuring and synergizing inputs from both public and private sensor sources and directly interoperable with HLS (harmonized Landsat Sentinel) surface reflectance products. ii) Sentinel-1 (S1) imagery, which contains 3 channels in total: [VV, VH, ANGLE] where V and H stand for vertical and horizontal orientations, respectively, and ANGLE stores the angle of observation to the earth surface as described here. The data is collected in Interferometric Wide (IW) swath mode and it includes both ascending and descending orbit directions. and iii) Sentinel-2 (S2) imagery, which includes all L2A bands in the following order [B01, B02, B03, B04, B05, B06, B07, B08, B8A, B09, B11, B12]. The bands that have original spatial resolution of 20m and 60m are interpolated with a nearest-neighbour method to a 10m resolution. [[Paper]](https://openreview.net/forum?id=uUa4jNMLjrL) [[Github]](https://github.com/lukaskondmann/DENETHOR)

 
### Ancillary Crop Related Annotated Datasets

- Crop Deep <br />
  This is the resulting work of this [paper](https://www.mdpi.com/1424-8220/19/5/1058), according to which, the CropDeep dataset is available from the corresponding author by email.

- [PlantVillage Dataset - Healthy and Unhealthy leaf images](https://data.mendeley.com/datasets/tywbtsjrjv/1) <br />
  In this data-set, 39 different classes of plant leaf and background images are available.  The data-set containing 61,486 images. The authors used six different augmentation techniques for increasing the data-set size. The techniques are image flipping, Gamma correction, noise injection, PCA color augmentation, rotation, and Scaling.  <br /> 
  [[Paper]](https://arxiv.org/abs/1511.08060) [[GitHub]](https://github.com/spMohanty/PlantVillage-Dataset)
  
- [iCrop Dataset - Street-level Imagery for Crop Classification](http://www.nwatch.top:8085/icrop/) <br />
  It is the first large, public, multiclass road view crop photo datase, for the development of crop type detection with deep learning. [[Paper]](https://www.mdpi.com/1424-8220/21/4/1165)

### Other Annotated Datasets

- [Sen1Floods11](https://github.com/cloudtostreet/Sen1Floods11) <br />
  A surface water dataset including raw Sentinel-1 imagery and classified permanent water and flood water. This dataset consists of 4,831 512x512 chips covering 120,406 km2 and spans all 14 biomes, 357 ecoregions, and 6 continents of the world across 11 flood events.  <br />
  [[Paper]](https://openaccess.thecvf.com/content_CVPRW_2020/html/w11/Bonafilia_Sen1Floods11_A_Georeferenced_Dataset_to_Train_and_Test_Deep_Learning_CVPRW_2020_paper.html) [[GitHub]](https://github.com/cloudtostreet/Sen1Floods11)
  
- [Labeled SAR imagery dataset of ten geophysical phenomena from Sentinel-1 wave mode (TenGeoP-SARwv)](https://www.seanoe.org/data/00456/56796/) <br />
  The TenGeoP-SARwv dataset is established based on the acquisitions of Sentinel-1A wave mode (WV) in VV polarization. This dataset consists of more than 37,000 SAR vignettes divided into ten defined geophysical categories, including both oceanic and meteorologic features. These images cover the entire open ocean and are manually selected from Sentinel-1A WV acquisitions in 2016. For each image, only one prevalent geophysical phenomena with its prescribed signature and texture is selected for labeling. The SAR images are processed into a quick-look image provided in the formats of PNG and GeoTIFF as well as the associated labels. They are convenient for both visual inspection and machine-learning-based methods exploitation.
  
- [Hand Labelled Crop/No-Crop dataset](https://zenodo.org/record/4680394#.YM85pm6EZpQ)  <br />
  This dataset provides the hand-labelled crop / non-crop points used for training, which were created by labelling high-resolution satellite imagery in QGIS and Google Earth Pro. Data is available for Ethiopia, Sudan, Togo and Kenya. [[Paper]](https://openaccess.thecvf.com/content/CVPR2021W/EarthVision/html/Tseng_Learning_To_Predict_Crop_Type_From_Heterogeneous_Sparse_Labels_Using_CVPRW_2021_paper.html) [[Github]](https://github.com/nasaharvest/crop-maml). 
    
- [Open VHR images and geospatial data (Netherlands)](https://nationaalgeoregister.nl/) <br />
  The National Georegister focuses primarily on the professional user. This can be a Geo- ICT specialist looking for datasets, services or other geo-information elements. But also a policy officer who wants to consult a map, a web developer or a student who develops a website or application and is looking for geo-information for it. Some example of available Datasets are:
  - [Land Parcel Identification System (LPIS)](http://nationaalgeoregister.nl/geonetwork/srv/eng/catalog.search#/metadata/b812a145-b4fe-4331-8dc6-d914327a87ff)
  - [Reference Parcels](https://www.nationaalgeoregister.nl/geonetwork/srv/eng/catalog.search;jsessionid=38BDD1EC9752E053336C3A2B28851B8B#/metadata/4fa03182-df71-4c39-87da-e7d5c0b82d88)
  - [Orthoimages (Web service)](https://www.nationaalgeoregister.nl/geonetwork/srv/eng/catalog.search#/map?facet.q=keyword%2Flandelijke%2520voorziening%2520beeldmateriaal&resultType=details&sortBy=relevance&any=Luchtfoto&fast=index&_content_type=json&from=1&to=50)
  - [Lidar data (Current Altitude Data)](https://www.nationaalgeoregister.nl/geonetwork/srv/eng/catalog.search#/metadata/41daef8b-155e-4608-b49c-c87ea45d931c)
  - [Soil Data(physical characteristics)](https://www.wur.nl/nl/show/Bodemfysische-Eenhedenkaart-BOFEK2020.htm)
  - [VHR Satellite Data](https://satellietdataportaal.nl/) Note: It is only accessible from within The Netherlands.
  
- [Land Cover Map (Korean Ministry of Environment)](https://egis.me.go.kr/main.do) <br />
  Korean Ministry of Environment provides three types of land cover map(level-1, level-2, level-3) according to its scale. Level-3 land cover map, the most detailed product, provides approximately 1m resolution by interpreting aerial photo(0.25m), Kompsat-2(1m) and Kompsat-3(0.7m) satellite images. It classifies 7 major land covers (Used area, Agricultural Area, Forest, Grassland, Wet land, Bareland, Water) and subdivides them into 41 classes. The level-3 product was produced at each province with several years of interval until 2018, and the most recent product was released at 2019 covering the entire nation with the imageries of 2018. 
The data is available only for the registered domestic researchers. Therefore, please ask for cooperation to the Korean researcher in order to use it for the research. 
   - Level-1 product: 30m resolution, raster format
   - Level-2 product: 5m resolution, shape format
   - Level-3 product: 1m resolution, shape format

- [Farm Map (Korean Ministry of Agriculture, Food and Rural Affairs)](http://data.nsdi.go.kr/dataset/20210707ds00001) <br />
  Korean Ministry of Agriculture, Food and Rural Affairs(MAFRA) provides farm map, which was produced by a visual interpretation on aerial photos and satellite images based on the parcel boundary of national GIS data. It classifies 6 major parcel types (Rice paddy, Field, Orchard, Cultivation structure, Ginseng, Fallow ground). The dataset was produced at different year for each administration boundary. 
The data is available only for the registered domestic researchers. Therefore, please ask for cooperation to the Korean researcher in order to use it for the research. 

### Web Application / Websites with labelled data
 
- [Mapillary Street Level Images](https://www.mapillary.com/) <br />
  A web platform/application where crowdsourced map data and street level imagery are available to everyone. Computer vision is used to combine those images and create immersive street-level views. Among many other features, Mapillary offers:
  - A quite extended coverage for Europe
  - Integration with OpenStreetMap, ArcGIS tools, and HERE Map Creator
  - The ability to request imagery for areas that, either don’t already have images, or just to get a more recent version of them
  - Navigation in a Google Street View style for easy visual interpretation
  - Filter imagery by capture time
  - Filter imagery by the types of objects that appear in the images (not an extended list of agriculture-specific objects yet though - mainly focused on city infrastructure and traffic lights/signs for now)

- [Eden Library](https://edenlibrary.ai/datasets) <br />
  Eden Library is a collection of high value plant datasets embedding agricultural domain knowledge produced in an academic environment. Eden Library includes a wide range of agrifood datasets such as:
    - Plant pests
    - Plant diseases
    - Weeds
    - Healthy plants  <br />
That were acquired using:
    - Various styles (Proximal, UAV upon request)
    - Various sensors (RGB, thermal, multispectral & hyperspectral upon request) <br/>
    [[GitHub]](https://github.com/Eden-Library-AI/eden_library_notebooks)
  
### UAV/Aerial imagery  

- [Open Aerial Map - UAV Imagery](https://map.openaerialmap.org/#/-18.6328125,18.562947442888312,3?_k=ir0sq6) <br />
  OpenAerialMap (OAM) is a set of tools for searching, sharing, and using openly licensed satellite and unmanned aerial vehicle (UAV) imagery. [[GitHub]](https://github.com/hotosm/OpenAerialMap)
  
- [VisDrone dataset](https://github.com/VisDrone/VisDrone-Dataset) <br />
  From the description of the dataset repository: Drones, or general UAVs, equipped with cameras have been fast deployed to a wide range of applications, including agricultural, aerial photography, fast delivery, and surveillance. Consequently, automatic understanding of visual data collected from these platforms become highly demanding, which brings computer vision to drones more and more closely. We are excited to present a large-scale benchmark with carefully annotated ground-truth for various important computer vision tasks, named VisDrone, to make vision meet drones. The VisDrone2019 dataset is collected by the AISKYEYE team at Lab of Machine Learning and Data Mining , Tianjin University, China. The benchmark dataset consists of 288 video clips formed by 261,908 frames and 10,209 static images, captured by various drone-mounted cameras, covering a wide range of aspects including location (taken from 14 different cities separated by thousands of kilometers in China), environment (urban and country), objects (pedestrian, vehicles, bicycles, etc.), and density (sparse and crowded scenes). Note that, the dataset was collected using various drone platforms (i.e., drones with different models), in different scenarios, and under various weather and lighting conditions. These frames are manually annotated with more than 2.6 million bounding boxes of targets of frequent interests, such as pedestrians, cars, bicycles, and tricycles. Some important attributes including scene visibility, object class and occlusion, are also provided for better data utilization.
  [[Paper]](http://128.84.4.34/abs/2001.06303) [[GitHub]](https://github.com/VisDrone/VisDrone-Dataset)

- [Agriculture-Vision: Challenges & Opportunities for Computer Vision in Agriculture](https://www.agriculture-vision.com/agriculture-vision-2021/dataset-2021) <br />
   Labelled images with 9 different classed; background, double_plant, drydown, endrow, nutrient_deficiency, planter_skip,water, waterway, weed_cluster. [[Paper]](https://openaccess.thecvf.com/content_CVPR_2020/html/Chiu_Agriculture-Vision_A_Large_Aerial_Image_Database_for_Agricultural_Pattern_Analysis_CVPR_2020_paper.html) [[GitHub]](https://github.com/SHI-Labs/Agriculture-Vision)

- [AU-AIR Dataset](https://bozcani.github.io/auairdataset) <br />
   AU-AIR dataset is the first multi-modal UAV dataset for object detection.
It meets vision and robotics for UAVs having the multi-modal data from different on-board sensors, and pushes forward the development of computer vision and robotic algorithms targeted at autonomous aerial surveillance.
AU-AIR has several features: <br />
    - Object detection in aerial images
    - more than 2 hours raw videos
    - 32,823 labelled frames
    - 132,034 object instances
    - 8 object categories related to traffic surveillance
    - Frames are also labelled with time, GPS, IMU, altitude, linear velocities of the UAV
[[Paper]](https://arxiv.org/abs/2008.02834) [[GitHub]](https://github.com/bozcani/auairdataset)

- [UAV-based Multispectral & Thermal dataset for exploring the diurnal variability, radiometric & geometric accuracy for precision agriculture](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/RYA2ZQ) <br />
To explore the diurnal variations, radiometric and geometric accuracy of UAV-based data for precision agriculture, a comprehensive dataset was created in a one-day field campaign (21 June 2017). The multi-sensor data set covers wheat, barley & potato experimental fields, located in Wageningen University and Research (WUR) farm maintained by Unifarm. UAV-based images were collected with several sensors over the experimental area, starting from 7:25am and ending at 20:00pm local solar time. The dataset consists of images collected by 9 flights with senseFly MSP4C, 9 with Parrot Sequoia, 2 with Slant Range P3, 5 with DJI Zenmuse X3 NIR, 4 with the senseFly Thermo-map and 1 with the RGB Sony WX-220. Additionally, validation measurements at radiometric calibration plates and plant sample locations were taken with a Cropscan handheld spectrometer and a tec5 Handyspec spectrometer. The dataset consists of the validation measurements, the raw images and the processed orthomosaics (both with and without geometric correction). <br />
[[Paper]](https://www.researchgate.net/profile/Ramin-Heidarian-Dehkordi/publication/340853010_UAV-based_Multispectral_Thermal_dataset_for_exploring_the_diurnal_variability_radiometric_geometric_accuracy_for_precision_agriculture/links/5f4bc8cda6fdcc14c5e9763c/UAV-based-Multispectral-Thermal-dataset-for-exploring-the-diurnal-variability-radiometric-geometric-accuracy-for-precision-agriculture.pdf) [[GitHub]]()

- [senseFly Datasets](https://www.sensefly.com/education/datasets/) <br />
Explore how senseFly drone solutions are employed around the globe — from topographic mapping and site surveys to stockpile monitoring, crop scouting, earthworks, climate change research and much more. The main domains that are included in this dataset are: <br />
   - Tactical Mapping
   - Surveying & Mapping
   - Mining, Quarries & Aggregates
   - Engineering & Construction
   - Agriculture
   - Environmental Monitoring
   - Humanitarian 

- [A Crop/Weed Field Image Dataset (CWFID)](https://github.com/cwfid/dataset/releases)
The Crop/Weed Field Image Dataset (CWFID) accompanies the following publication: "Sebastian Haug, Jörn Ostermann: A Crop/Weed Field Image Dataset for the Evaluation of Computer Vision Based Precision Agriculture Tasks, CVPPP 2014 Workshop, ECCV 2014"
This dataset comprises field images, vegetation segmentation masks and crop/weed plant type annotations. The paper provides details, e.g. on the field setting, acquisition conditions, image and ground truth data format.
[Paper](https://link.springer.com/chapter/10.1007/978-3-319-16220-1_8) [Github](https://github.com/cwfid/dataset)

### Crop phenology annotated dasets
- [DWD_RECENT](https://opendata.dwd.de/climate_environment/CDC/observations_germany/phenology/annual_reporters/crops/) <br />
 DWD Climate Data Center (CDC): Phenological observations of crops from sowing to harvest, in Germany. The temporal coverage is rolling, with a window of 500 days (ending always yesterday), the soatualk  and the crops of interest are: meadows, winter wheat, winter rye, winter barley, winter oilseed rape, summer wheat, spring barley, oat, sunflower, maize, beet, sugar beet, fodder beet. For more information click [here](https://opendata.dwd.de/climate_environment/CDC/observations_germany/phenology/annual_reporters/crops/recent/DESCRIPTION_obsgermany-phenology-annual_reporters-crops-recent_en.pdf).
 
 - [DWD_ARCHIVE](http://www.pep725.eu/data_download/data_selection.php) <br />
 DWD Climate Data Center (CDC): Historical phenological observations of crops from sowing to harvest, in Germany. It contatins data from 1951-01-01 until 2017-12-31 for dozins of crops (meadows, winter wheat, winter rye, winter barley, winter oilseed rape, summer wheat, spring barley, oat, sunflower, maize, potato, early potato (pregerminated), early potato (non pregerminated), late potato, green
bean, green pea, tomato, white cabbage, alfalfa, red clover, beet, sugar beet, fodder beet). For more information click [here](https://opendata.dwd.de/climate_environment/CDC/observations_germany/phenology/annual_reporters/crops/historical/DESCRIPTION_obsgermany-phenology-annual_reporters-crops-historical_en.pdf).
 
 - [PEP725](https://opendata.dwd.de/climate_environment/CDC/observations_germany/phenology/annual_reporters/crops/) <br />
 The main objective of PEP725 is to promote and facilitate phenological research by delivering a pan European phenological database with an open, unrestricted data access for science, research and education ([datapolicy](http://www.pep725.eu/downloads/PEP725_Data_Use_Policy_201805.pdf)). [Paper](https://doi.org/10.1007/s00484-018-1512-8)
 

### European projects 
- [NextGEOSS Data Catalog (DaaS)](https://catalogue.nextgeoss.eu/)
  - Archived data: YES
  - Real Time data or NEAR REAL TIME: YES
  - Data harvesting policy: Initially driven by the needs of the pilots, now opened to all European project. 
  - Data are accessible via an Opensearch standard API with OGC Opensearch GEO and Time Extensions (http://www.opengeospatial.org/standards/opensearchgeo) 
  - The Catalog GUI allows generating the requests that can be then be reused in a M2M dialogue. Compliancy has been validated with NASA Validation tools.

- [Geocradle Data Catalog (DaaS)](http://datahub.geocradle.eu/search/type/dataset)
  - GEO-CRADLE PILOT 1 datasets: Adaptation to Climate Change (ACC): ACC-DUST
  - GEO-CRADLE PILOT 2 datasets: Improved Food Security – Water Extremes Management (IFS-WEM): Regional Soil Spectral Library
  - GEO-CRADLE PILOT 3 datasets: Access to Raw Materials (ARM)
  - The Regional Data Hub provides access to millions of regional datasets, and thus fosters further data sharing and EO service development for the benefit of the relevant science and geo-information sector. It includes 26.623.346 datasets and keeps growing.

- Copernicus
  - [COPERNICUS ATMOSPHERE MONITORING SERVICE : CAMS](https://atmosphere.copernicus.eu/) 
  - [COPERNICUS CLIMATE CHANGE SERVICE : C3S](https://climate.copernicus.eu/)
  - [COPERNICUS LAND MONITORING SERVICE : CLMS](https://land.copernicus.eu)
  - [COPERNICUS MARINE ENVIRONMENT MONITORING SERVICE: CMEMS](https://marine.copernicus.eu)
  - [COPERNICUS OPEN ACCESS HUB](https://scihub.copernicus.eu/dhus/#/home)

## Other Useful Data Collections
- [Radiant MLHub](https://mlhub.earth/datasets)
- [Awesome-Remote-Sensing-Dataset](https://github.com/zhangbin0917/Awesome-Remote-Sensing-Dataset)
- [awesome-remote-sensing](https://github.com/attibalazs/awesome-remote-sensing)
- [Awesome Remote Sensing Change Detection](https://github.com/wenhwu/awesome-remote-sensing-change-detection)
- [Remote sensing resources](https://github.com/jqtrde/remote)


