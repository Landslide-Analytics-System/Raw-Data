# Weather Data

## Structure

There are 6011 folders containing data for 6011 landslides that took place between -10 to 40 degrees North and 60 to 150 degrees East (Southern and Eastern Asia)

The name of each folder is the FID of each landslide, as found in [Global_Landslide_Catalog.csv](https://github.com/Landslide-Analytics-System/Data/blob/main/Global_Landslide_Catalog.csv)

Each folder corresponds to a landslide. In each folder is `info.txt`, a description of the landslide, and 36 XML files containing weather data from 35 days before
the landslide up to the day of the landslide.

```
<Landslide FID>/
├── info.txt (description of landslide)
├── <day_of_landslide.xml>.xml 
├── <day_before_landslide.xml>.xml
├── ..... (33 files)
└── <5_weeks_before_landslide.xml>.xml
```

## Features
- Precipitation
- Temperature
- Humidity
- Wind Speed
- Air Pressure
- Visibility
- More Info

Data is collected every 3 hours for each date (each XML file has information for 8 different times)
