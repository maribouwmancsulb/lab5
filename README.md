# Computer Vision in Remote Sensing

## Land-Use and Land-Cover Change Detection

### Introduction

One of the most typical uses of remote sensing is to analyze changes of land cover and land use. Land cover refers to the physical characteristics of the earth’s surface while land use refers to anthropogenic activities, or the utilization, associated with a piece of land. Land use/land cover (LULC) change detection is important for understanding how land changes over time. Studying LULC change is inherently multidisciplinary and can provide information for many different fields. For example, LULC change analysis can be used in measuring environmental degradation, managing natural resources, or monitoring climate change. 

Studies either compare two images that are taken years apart or analyze a series of images to assess rates of change over time. Most LULC change analyses follow a similar process: obtaining multi-temporal satellite imagery/remotely sensed images, processing and classifying the imagery, and calculating the differences between images. The classification component of this process is one of the techniques associated with computer vision. Computer vision involves machines using algorithms and methods to interpret images similarly to how a human would, which is an essential component when studying LULC changes. 

Research studies have been conducted across different countries to measure changes in urban areas, agricultural lands, forested regions, etc. The primary object of these studies is to create a time series of LULC and examine the scope and rates of these changes. Understanding how LULC change occurs is important for identifying the driving factors. A study in Fez, Morocco was aimed at calculating the change in impervious surfaces in comparison to the city’s population growth. Researchers in Mekelle, Ethiopia assessed the ecological changes of the city and its environs to understand the spatiotemporal dynamics associated with the city’s rapid development. Below is a table of the land LULC types for Mekelle and the classification results.

![image](https://user-images.githubusercontent.com/127627133/234779767-4869b1b6-261d-49c8-a134-ebfc95085258.png)
![image](https://user-images.githubusercontent.com/127627133/234779797-bc8fed15-2795-481a-9d22-1acc7b0cdc59.png)


### Methodology

Many studies utilize imagery obtained from the Landsat satellites: Thematic Mapper (TM), Enhanced Thematic Mapper Plus (ETM+), and Operational Land Imager (OLI) and Thermal Infrared Sensor (TIRS). Landsat imagery is beneficial for its synoptic view, selection of cloud-free images, and wide temporal range. Additionally, Landsat images have a medium resolution (30m), are cost effective, and are GIS compatible. After the data and imagery is obtained, images are classified using GIS processing software (such as the ERDAS Imagine software). A common method for computer vision classification is the maximum likelihood supervised classification (MLC). With MLC, the user provides training standards to the machine to complete image classification. MLC is used to calculate the area of different land covers or index images. Classification results can be combined with topographical maps, aerial photographs, field observations, or ground control points. Below is the pre- and post-classification imagery (1984 and 2013) for Fez.  

False color composites of Landsat images             |  Land cover maps from classification
:-------------------------:|:-------------------------:
![image](https://user-images.githubusercontent.com/127627133/234781132-83e5ff53-0e7c-4b36-a81e-04b6d2a1bdb0.png)  |  ![image](https://user-images.githubusercontent.com/127627133/234781195-78c43a83-e148-4202-86fb-194f0d65a8ae.png)


### Conclusion

Scientists often bolster their classification results with an accuracy assessment to quantify the precision of the computer vision output. Improving computer vision and classification techniques is important to accurate monitoring and assessment of land change. LULC change analyses will become essential for environmental science investigations as well as policy decisions. 

### References

“Application of Remote Sensing in Land Cover and Land Use Mapping.” GISOutlook, 17 May 2022, https://gisoutlook.com/2020/05/application-of-remote-sensing-in-land-cover-and-land-use-mapping.html.

Canada, Natural Resources. “Land Cover & Land Use.” Natural Resources Canada, / Gouvernement Du Canada, 20 Nov. 2015, https://natural-resources.canada.ca/maps-tools-and-publications/satellite-imagery-and-air-photos/tutorial-fundamentals-remote-sensing/educational-resources-applications/land-cover-biomass-mapping/land-cover-land-use/9373.

El Garouani, Abdelkader, et al. “Analysis of Urban Growth and Sprawl from Remote Sensing Data: Case of Fez, Morocco.” International Journal of Sustainable Built Environment, vol. 6, no. 1, 10 Feb. 2017, pp. 160–169., https://doi.org/10.1016/j.ijsbe.2017.02.003. 

Fenta, Ayele Almaw, et al. “The Dynamics of Urban Expansion and Land Use/Land Cover Changes Using Remote Sensing and Spatial Metrics: The Case of Mekelle City of Northern Ethiopia.” International Journal of Remote Sensing, vol. 38, no. 14, 13 Apr. 2017, pp. 4107–4129., https://doi.org/10.1080/01431161.2017.1317936.   
