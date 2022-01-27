# Health and pollution attribution framework  

The goal of this project is to connect individual health measures with geographically localized sources of pollution. 

## Data  

Three types of data are needed: neighbourhood level pollution maps, individual health measures, and individual location coordinates.   

### Pollution maps (time series, geospatial)   

#### Purple Air  

Analysis tutorial: https://publiclab.org/notes/jiteovien/08-28-2018/download-analyze-your-purple-air-data    

Example data: https://www.purpleair.com/sensorlist?exclude=true&nwlat=49.35544245180316&selat=49.18272278053968&nwlng=-123.20327344394512&selng=-122.77343335605468&sensorsActive2=604800 

Another tutorial: https://www.youtube.com/watch?v=b-KXGvng7m8   

Example review: https://publiclab.org/notes/bhamster/01-05-2021/wrapping-up-an-air-quality-research-area-review  

### Invidiual health data (time series, scalar)  

#### Heart rate  

Smoke inhalation should be correlated with changes in heart rate, mainly as a confirming measure of the location and smoke map data.

#### Sleep quality  

Changes in sleep quality correlated with smokier days, could be a measure that connects to changes in income the following day.  

#### Miscellaneous disease growth rates  

Addition columns to manually enter measurements of some of other health indicator, like changes in tumour size betweem two dates. 

### Individual location data (time series, geospatial)

#### Own tracks  

GPS data logged from Android/ios devices - https://github.com/owntracks   

## Modeling  

Detection and attribution can be thought of as multiple regression, where the outcome variable is a health outcome, but the range of the input predictors are estimated by something more like a numeric process model (think global climate simulation, where the input parameters have themselves been estimated for a set simulations). - https://arxiv.org/pdf/2012.04200.pdf  

### PyDna  
"Detection and Attribution framework in python using the Optimal Fingerprinting Approach (Hasselmann, 1993; Ribes et al. 2013)" - 
https://github.com/pinplex/PyDnA.git    

### Possible package file to a city simulator  

Would need a city simulator that provides an API for citizens to be modeled with the right distributions.

## Legal precedents    
 - https://decisions.civilresolutionbc.ca/crt/crtd/en/item/484448/index.do?q=Wood+smoke  
 - https://web.archive.org/web/20080705112031/http://www.woodburnersmoke.net/  
