# Multistate In-situ Sensor Testbeds (MIST)

The goal of the project is to deploy soil moisture testbeds across multiple states to evaluate, calibrate, and disseminate existing and emerging research-grade and consumer-grade in-situ sensing technologies.

This is a collaborative project among four U.S. institutions:

- Andres Patrignani and Nathaniel Parker (Postdoc), Soil Water Processes, Department of Agronomy, Kansas State University
- Briana Wyatt and Seyed Ali Azizi (PhD student), Soil Physics, Department of Soil and Crop Sciences, Texas A&M
- Michael Cosh, Hydrology and Remote Sensing Laboratory, USDA-ARS, Beltsville, MD
- Tyson Ochsner and Jerry Brown (PhD student), Soil Physics, Department of Plant and Soil Sciences, Oklahoma State University

The project is supported by the United State Department of Agriculture (USDA) Natural Resources Conservation Service (NRCS) through award #NR213A750025C007 and the USDA National Institute of Food and Agriculture (NIFA) through multi-state project W4188.

Testbed data pre-processing:

Regarding Texas A&M University data, it was processed before being published to the public. For the volumetric water content data, the lower and upper thresholds were set at 0.0 and 0.6 cm³/cm³, respectively, meaning the values were set to NaN for dates when the data fell outside these thresholds. Additionally, on some days, the batteries died, and no data was recorded. For those days, NaN values were inserted into the dataset to maintain a continuous time series. In some cases, when the battery was recharged after having died, the date was reset to the year 2000 because the data logger's internal battery could not keep the date updated during the period the external battery was dead. For those days, the time was reset after collecting the data in the field, and a backward time series was created from the date when the time was reset in the field to correct all incorrect dates (note that this happened only for Site 1). Furthermore, all duplicate dates were also removed from the datasets.
