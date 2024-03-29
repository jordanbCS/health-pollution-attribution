# Health and pollution attribution framework  

The goal of this project is to connect individual health measures with geographically localized sources of pollution. 

## Data  

Three types of data are needed: neighbourhood level pollution maps, individual health measures, and individual location coordinates.   

### Pollution maps (time series, geospatial)   

#### Purple Air  

Analysis tutorial: https://publiclab.org/notes/jiteovien/08-28-2018/download-analyze-your-purple-air-data    

Example data: https://www.purpleair.com/sensorlist?exclude=true&nwlat=49.35544245180316&selat=49.18272278053968&nwlng=-123.20327344394512&selng=-122.77343335605468&sensorsActive2=604800 

Tutorial: https://www.youtube.com/watch?v=b-KXGvng7m8   

Example use: https://publiclab.org/notes/bhamster/01-05-2021/wrapping-up-an-air-quality-research-area-review  

### Invidiual health data (time series, scalar)  

#### Heart rate  

Example: Smoke inhalation correlated with changes in heart rate, mainly as a confirming measure of the location and smoke map data.

#### Sleep quality  

Example: Changes in sleep quality correlated with smokier days, could be a measure that connects to changes in income the following day.  

#### Miscellaneous disease growth rates  

Additional columns to manually enter health measures, e.g., tumour size over time. 

### Individual location data (time series, geospatial)

#### Own tracks  

GPS data logged from Android/ios devices - https://github.com/owntracks   

## Modeling  

Detection and attribution as multiple regression: predicted variable is a health outcome, and predictors are estimated by something like a numeric process model (think global climate simulation, where the input parameters have themselves been estimated for a set simulations). - https://arxiv.org/pdf/2012.04200.pdf  

### PyDna  
"Detection and Attribution framework in python using the Optimal Fingerprinting Approach (Hasselmann, 1993; Ribes et al. 2013)" - 
https://github.com/pinplex/PyDnA.git    

### Possible package file to a city simulator  

Would need a city simulator that provides an API for citizens to be modeled with the right distributions.

## Existing related monetary scales and valuations  

 - "Health Impact Scale for Air Quality Improvements in the Canadian Lower Fraser Valley Airshed" - restrictions on wodd burning appliances is valued at $438M/per year in Metro Vancouver (2019).
   - http://www.metrovancouver.org/services/air-quality/AirQualityPublications/HealthImpactScaleforAirQualityImprovementsintheCanadianLowerFraserValleyAirshed.pdf  

## Related projects  

 - Link has been removed but this alluded to a global real time pollution map: https://www.reddit.com/r/ClimateOffensive/comments/vm3ju2/i_have_created_a_web_visualization_that_shows_for/    

## Other  

Data sources and refence material page like this: https://earth.nullschool.net/about.html   

## Legal precedents   

 - A Mystery in the Air --- SCIENCE VS: https://gimletmedia.com/shows/science-vs/94hxnjn    
   - "Global first as British girl’s death certificate lists air pollution as a cause of death
18 December 2020, London: In what is believed to be a global first, Deputy Coroner Phillip Barlow ruled on Wednesday that Ella Adoo-Kissi-Debrah, a 9 year-old girl who lived just 25m from the South Circular in South London, died in February 2013 as a direct result of air pollution...Reading aloud his verdict, Philip Barlow said that he believed air pollution made a “material contribution to Ella’s death”. She was exposed to levels of nitrogen dioxide and particulate matter in excess of World Health Organisation guidelines. The level of air pollution she was exposed to was therefore excessive. The principal source of her exposure was traffic emissions." https://chambers.com/articles/extraordinary-landmark-inquest-rules-air-pollution-contributed-to-death-of-ella-adoo-kissi-debrah   
 - https://decisions.civilresolutionbc.ca/crt/crtd/en/item/484448/index.do?q=Wood+smoke  
 - https://web.archive.org/web/20080705112031/http://www.woodburnersmoke.net/  

