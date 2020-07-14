# **Eurosat-Project**

Sentinel-2 is an Earth observation mission from the Copernicus Programme that systematically acquires optical imagery at high spatial resolution (10 m to 60 m) over land and coastal waters. The mission is a constellation with two twin satellites, Sentinel-2A and Sentinel-2B.

* The mission supports a broad range of services and applications such as agricultural monitoring, emergencies management, land cover classification or water quality.

* Sentinel-2 has been developed and is being operated by ESA, and the satellites were manufactured by a consortium led by Airbus DS.

* The  aim  of  land  use and land cover classification is to automatically provide labels describing  the  represented  physical  land  type  or  how  a  land area is used (e.g., residential, industrial). 

* EuroSAT  dataset  consists  of  **27,000**  labeled  images  with  10 different land use and land cover classes.

* Sentinel-2A  is one  satellite  in  the  two-satellite  constellation  of  the  identical land  monitoring  satellites  Sentinel-2A  and  Sentinel-2B.  The satellites  were  successfully  launched  in  June  2015  (Sentinel-2A)  and  March  2017  (Sentinel-2B).   

* The  two-satellite  constellation generates a coverage of almost the entire Earth’s land surface about every five days.

To  construct  an  image classification dataset, we performed the following two steps:
1. Satellite Image Acquisition: We gathered satellite images of  European  cities  distributed  in  over  34  countries.

2. Dataset Creation: Based on the obtained satellite images, we created a dataset of 27,000 georeferenced and labeled image patches. The image patches measure 64x64 pixels and have been manually checked. 

The  covered  cities  are  distributed  over  the  34  Euro-pean  countries:  **Austria,  Belarus,  Belgium,  Bulgaria,  Cyprus,Czech Republic (Czechia), Denmark, Estonia, Finland, France,Germany, Greece, Hungary, Iceland, Ireland, Italy / Holy See,Latvia,  Lithuania,  Luxembourg,  Macedonia,  Malta,  Republicof Moldova, Netherlands, Norway, Poland, Portugal, Romania, Slovakia, Slovenia, Spain, Sweden, Switzerland, Ukraine and United Kingdom.**

In  order  to  **improve**  the  chance  of  getting  valuable  image patches,  we  selected  satellite  images  with  a  low  cloud  level. Besides the possibility to generate a cloud mask, ESA provides a cloud level value for each satellite image allowing to quickly select  images  with  a  low  percentage  of  clouds  covering  theland scene. 

We  have  chosen  10  different and use and land cover classes based on the principle that theyshowed to be visible at the resolution of 10 meters per pixel.

**Aplications:**
1. Land Use and Land Cover Change Detection
2. Assistance in Mapping
3. Deforestation is a main contributor to climate change, therefore the detection of deforested land isof particular interest (e.g., to notice illegal clearing of forests). 


<table>
  <tr><td>
    <img src="https://github.com/pauldamsa/Eurosat-Project/blob/master/Bolivia.png"
alt="Fashion MNIST sprite"  length = "1500" width="1500">
  </td></tr>
  <tr><td align="center">
    <b>Change detection application: The left image was acquired near Villamontes, Bolivia in October 2015. The right image was acquired in the same area in September 2016 showing that a large land area has been defore
  </td></tr>
</table>

<table>
  <tr><td>
    <img src="https://github.com/pauldamsa/Eurosat-Project/blob/master/Dallas.png"
alt="Fashion MNIST sprite"  length = "1500" width="1500">
  </td></tr>
  <tr><td align="center">
    <b> Change detection application: The left image was acquired in the surroundings of Dallas, USA in August 2015 showing no dominant residential area in the highlighted area. The right image was acquired in the same area in March 2017. The system classified the area as residential showing that a residential area has been built up. 
  </td></tr>
</table>

<table>
  <tr><td>
    <img src="https://github.com/pauldamsa/Eurosat-Project/blob/master/Shanghai.png"
alt="Fashion MNIST sprite"  length = "1500" width="1500">
  </td></tr>
  <tr><td align="center">
    <b> The left image was acquired in the surroundings of Shanghai in December 2015 showing an area classified as industrial. The right image shows the same region in December 2016 revealing that the industrial buildings have been demolished.
  </td></tr>
</table>

<table>
  <tr><td>
    <img src="https://github.com/pauldamsa/Eurosat-Project/blob/master/mistagged%20%20areas.png"
alt="Fashion MNIST sprite"  length = "1500" width="1500">
  </td></tr>
  <tr><td align="center">
    <b> A patch-based classification system can verify already tagged areas, identify mistagged areas or bring large area tagging as shown in the above images and maps. The left Sentinel-2 satellite image was acquired in Australia in March 2017. The right satellite image was acquired in the surroundings of Shanghai, China in March 2017. The corresponding up-to-date mapping images from OpenStreetMap show that the industrial areas in the left satellite image are almost completely covered (colored gray). However, the industrial areas in the right satellite image are not properly covered. 
  </td></tr>
</table>

<table>
  <tr><td>
    <img src="https://github.com/pauldamsa/Eurosat-Project/blob/master/piechart_dist_images.png"
alt="Fashion MNIST sprite"  length = "1500" width="1500">
  </td></tr>
  <tr><td align="center">
    <b> EuroSAT  dataset  distribution.  The  georeferenced  images are distributed all over Europe. The distribution is influenced by the number of represented cities per country in theEuropean Urban Atlas 
  </td></tr>
</table>

EuroSAT: A Novel Dataset and Deep Learning Benchmark for Land Use and Land Cover Classification. Available from: https://www.researchgate.net/publication/319463676_EuroSAT_A_Novel_Dataset_and_Deep_Learning_Benchmark_for_Land_Use_and_Land_Cover_Classification 
