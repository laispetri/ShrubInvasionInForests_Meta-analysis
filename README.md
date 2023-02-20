# ShrubInvasionInForests_Meta-analysis
---

This code allow readers to run models to reproduce results and figures of the paper "Assessing the mechanisms and impacts of shrub invasion in forests: a meta-analysis", currently submitted to Journal of Applied Ecology.


## Description of the data and file structure

Code was build in RMarkdown. All packages needed are listed in the beginning of code, along with extra information on how to organize folder within the working directory. 

You will need five CSV files, access information below.

- "Data.csv": StudyIDOriginal = unique study identifier (integer), ObsIDOriginal = unique observation identifier (integer), Lat_m = latitude in degrees where the data was collected (double), Long_m = longitude in degrees where the data was collected (integer), Continent = the continent where the data was collected (character), Country = the country where the data was collected (character), Province_Region = province, region, state, or county where the data was collected (character), City = city (or the nearest city to the study site) where the data was collected (character), OlsonEtAl2001_GlobalEcoregions = global ecoregions where the data was collected (character), Elevation_m = elevation in meters of where the data was collected (integer), Precipitation_mm = or rainfall (mm), total annual precipitation where the data was collected (double), JanuaryTemp_C = mean January temperature in degrees Celsius (double), JulyTemp_C = mean July temperature in degrees Celsius (double), MeanAnnualTemp_C = mean annual temperature in degrees Celsius (double), ForestCommunity = defines the forest community type (character, multiple categories), TypeOfForest = defines the forest type with regard to history of exploration and/or current use (character, multiple categories), TypeOfStudy = specifies the general method of data collection (character; field experiment, greenhouse, or observational), Disturbance = occurence of disturbance [yes, no, not_reported] (character), NatureOfDisturbance = dummy variable of disturbance type (1 = natural, 2 = human, 3 = natural and human, NA = missign information, not_reported = when disturbance was indicated that existed but no specifics were given), YearOfDisturbance = year that the disturbance ceased (character), YearOfDataMeasurement = year or range of years that the data was collected (character), YearOfDataMeasurement_reported = specifies whether the article reported the year of data collection (character; yes, no), AccInvasiveSpecies = invasive species Latin name(s) standardized through the Taxonomic Name Resolution Service (character), CommInvasiveSpecies = common name for each invasive species as reported by the paper, or collected in online databases (character), InvasiveSpeciesOrigin = invasive species country/continent of origin as reported by the paper, or collected in online databases (character), MultipleInvader = multiple shrub invasive species present in the system (1) or not (0) (integer), Mechanism = mechanism by which invasion took place [1- propagule pressure, 2- empty niches, 3- low biotic resistance] (integer), NcontInv = sample size of invader response control [low invasion] (integer), NtreatInv = sample size of invader response treatment [high invasion] (ingeger), TypeOfResponse = specifies the performance metric (character), UnitOfResponse = specifies the unit of the performance metric (character), TypeOfMeasuredVariability = unit of variance metric reported associated with the mean performance value [SD, SE, and upper maximum value] (character), InvContmean = mean value of invader performance metric when forest understory was under low invasion levels (double), InvContsd = variance value of invader performance metric when forest understory was under low invasion levels (double), InvTreatmean = mean value of invader performance metric when forest understory was under high invasion levels (double), InvTreatsd = variance value of invader performance metric when forest understory was under high invasion levels (double), NativeResponse_CATEGORY = native community metrics in broad categories (character), NativeResponse_SUBCATEGORY = specifies/details the subcategories within each broad category (character), NativeCommunity = when biotic response, specifies whether the native response is at the community level (1) or species level (0) (integer), NcontNat = sample size for the native response control at low invasion levels (integer), NtreatNat = sample size for the native response treatment at high invasion levels (integer), TypeOfTreatment = defines the native response metric (character), UnitOfTreatment = specifies the unit of the native response metric (character), TypeOfMeasuredVariability_Response = unit of variance metric reported associated with the mean native response value [SD, SE, or upper maximum value] (character), NatContmean = mean value of native response metric at low invasion levels (double), NatContsd = variance value associated with the mean value of native response metric at low invasion levels (double), NatTreatmean = mean value of native response metric at high invasion levels (double), NatTreatsd = variance value associated with the mean value of native response metric at high invasion levels (double), SourceFromPapers = figure, table, or text section from where the data was extracted (character).

Details on the "Data.csv" file variables above can be found in the supplements of the paper.

- "InvEstimateRESULTS.csv": ObsIDOriginal = unique identifier for an observation (integer), ESInvmean = estimated mean effect size of invasive species performance (double), ESInvSD = estimated standard deviation of invasive species performance (double).

- "NatBioticEstimateRESULTS.csv": ObsIDOriginal = unique identifier for an observation (integer), ESNatmean = estimated mean effect size of native community performance (double), ESNatSD = estimated standard deviation of native community performance (double).

- "NatAbioticEstimateRESULTS.csv"": ObsIDOriginal = unique identifier for an observation (integer), ESNatmean = estimated mean effect size of abiotic features of the native community (double), ESNatSD = estimated standard deviation of abiotic features of the native community (double).

Cells with missing data are filled with NAs.

## Sharing/Access information

All five CSV files needed to run this code can be found in https://doi.org/10.5061/dryad.msbcc2g33.

Please, cite the original paper (once it is published) if using any data or code shared here.
