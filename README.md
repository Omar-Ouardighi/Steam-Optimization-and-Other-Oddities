# Steam-Optimization-and-Other-Oddities
Create a flexible model that can characterize steam growth in reservoirs using data from the South Belridge Field

## Challenge Description
Aera has been an active energy producer in California for the last 24 years.  Aera is always seeking new ways to more responsibly produce energy. One such initiative is to reduce the amount of input energy necessary to operate their oil fields. These oil fields have high viscosity oil that requires steam injection for production.  Aera Engineers are working to find opportunities to maintain production levels while reducing the amount of steam necessary and thus the energy needed to operate.

## Background
Aera’s method of hydrocarbon extraction is similar to methods developed elsewhere in the world with high viscosity oil.  For a good overview about the physical processes happening to produce the data please check out Zerkalove (2015).  If you have access to journal articles from the Society of Petroleum Engineers you can also review SPE 11219 and SPE 13348.

## Description of the Dataset
Contestants will be supplied a data table with all the necessary inputs to build a model.
![image](https://images.ctfassets.net/yr01c1s2xcnk/3m2nM6hsv9kfsjb1BmmHme/72f8b1eb5524cdc559809999237c9599/Aera_column_descriptions.JPG)
Some other considerations regarding this data:

    A “sand” is an individual layer.  A “reservoir” is a family of sands that are adjacent and have similar properties.
    Some sands may end before reaching an injector well which is why there are several NaN values for some of the columns. An NaN value means sand is not present.
    The distance from producing well to injectors is an important factor but instead of providing map locations, the dataset has relative distances between the nearest three injector wells.

Target Output
The target variable for this competition is the PCT_DESAT_TO_ORIG. Models should predict this variable. Additionally we welcome creative visualizations or other analyses as detailed in the Evaluation Criteria.
