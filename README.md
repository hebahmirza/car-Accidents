# car-Accidents
data analysis for car accidents in saudi arabia regions by python


Project 1: Local Traffic, Statistical Summaries and Inference

### Overview

This project include:
- basic statistics
- many Python programming concepts
- programmatically interacting with files and directories
- visualizations
- EDA
- working with Jupyter notebooks for development and reporting

**The link for Non-Technical report is in the link:
https://medium.com/@hebahmirza1/local-traffic-statistical-summaries-and-inference-in-saudi-arabia-5f0dc0ba2c48

**Data Sets:**

in this project, we will aim to find a clear pattern between the Traffic accedetns and the accedent's Regions in Saudi Arabia. Here also, well determine any other factors that could affect the accedents percentage and the type of casulties (Death/Insured).

By looking at the number of traffic accidents and driving licenses issued in Saudi Arabia, analysing the data and defining clear patterns between them, we must come out with clear findings that can reduce the number of accedents and casulties.
**Project Steps**
- read and import the two data sets into 1- traffic_accedents and 2-Drivint_licence
- view the datasets data, to start cleaning:
    - remove usless characters such as paranthess found around (Year), and n character in Value column, and separate 2d_geo_location into x y axes columns
    - convert object types (Year, No of Accedents, No of Insured casulties, No of Dead casulties, x y geo_location) to numeric types
    - Drop Nan rows ,and delete redundent columns such as Unnamed 0:, and Unnamed 1:0, and Values (after the merge)
- transform the long dataset traffic_accedent to wide form wide_traffic_accedent by pivot_table:
- Merged the new wide_traffic_accednts with the second dataset Drivint_Licence to (car_accedent_Licence_related)
- Provide visualization and statisics:
    - Heatmap represets the corollation between all columns of the merged dataset.
    - Bar, scatter and histograms

**Data Dictionary:**
|Feature|Type|Dataset|Description|
|---|---|---|---|
|Year|int|car_accedent_licence_related|year represting timing of incedents| 
|region|obj|car_accedent_licence_related|Saudi reagions|
|no_of_Accedents|int|car_accedent_licence_related|Number car_accedent_licence_relatedof car Accedents|
|Driving_Licence|int|car_accedent_licence_related|Number of Driving Licences issued|
|no_of_Insured_casult|int|car_accedent_licence_related|Number of Injared casulties|
|no_of_Dead_casult|int|car_accedent_licence_related|Number of Dead casulties|
|x_geo_loc|float|car_accedent_licence_related| x axes of geolocation of the insedent|
|y_geo_loc|float|car_accedent_licence_related| y axes of geolocation of the insedent|

**final conlcutions and findings**

The tow given datasets Traffic Aaccedents and Driving Licence were very usfel after beaing cleaned and joined together. 
Many fingings appeared during this project from statistics and figures plotting.
**First, the list of statistical analysis from this projct:**
- **The Minimum/ Max number of Accedents** is : 3,193/ 145,541 and the **mean** is : 38,877 Accedents
- **The Minimum/ Max number of Dead casulties** is: 112/2,243 and the **mean** is: 644 Dead
- **The Minimum/ Max number of Insured casulties** is: 374/12,383 and the **mean** is: 2,902 Insured
- **The Minimum/ Max number of Driving Licences issued** is: 2,153/495,307 and the **mean** is: 69,517 Driving licences issued.

- Najran has the minimum Driving licene issued in 2016 : 2,153
- Riyadh has the maximum Driving licence issued in 2017: 495,307
- the highest number of accedents in Makkah: 145,541 accedent happend in 2017.
- the lowest number of accedents in Najran:3,193 accedent happened in 2017

**More outcomes:**
The Regions that have more Driving Licenses issued in each year than the year average are 5 regions:* 
- Hail (2016-2017), Jazan (2017), Madinah(2016-2017), Makkah(2016-2017), Riyadh (2016-2017)

The Regions that have more Traffic Accidents happened in each year than the year average are 5 regions:
- Jazan(2016-2017), Madinah (2016-2017), Makkah(2016-2017),Riyadh(2016-2017), Tabuk (2016)

The datasets on plot, showed high value outler in
- The number of Driving licence issued in 2017, to 495,307 where the total average is only 16,085. And Riyadh was the region that reached this outlier.
- The maximum number of Injaries from car accedents by reagion was in Makkah, where it jumped to more than 12,000 Injaries, while the mean number among all reagins is only 2,980.
- Makkah reagion also, had the highest number of Dead casulties 2,243, and Riyadh had the second place where it had more than 800, even though the number of driving licences issued was the highes in Riyadh.
- Eventhough, the number of driving licence issued in 2017 was greater than 2016, but it seem's people began to take more care, so the number of Insured and Dead casulties was less in 2016.
 
**Final findings:**

From this data set, we need to find the relations and patterns between the data, to come up with usefall findings, that might reduce the number of Accedents, Injaries and Deaths from Car accedents. 
The project started by observing the two given data sets, cleaning them rearanging and grouping them, then merging them together. After the merge we started to conduct some statistical findings to retrive some usefall findings. Finally some plottings and visualilzation (heatmap, bar charts, histograms and scatters) was conducted to view the max min, mean, average values among all the given features.
we found that the maximum number of Driving licenses issued in Riyah, which hit a high oulier number. Evan that Hail region was also above the average; it wasnt icluded in the highes average range of accedetns in 2017. On the other hand, Tabouk region was ander the average regions issueing driving licences, but thier number of accedents was above the averange range.

The highest percentage of Accedents, Injaries, and Deaths appears to be in Makkah Region 2017, even though it was second after Riyadh region in number of Licences issued.
Najran region had the lowest licences issued and the lowest Accedents as well.
Finally, the most impact between data is the Number of Driving licences issued, it positively affects on :
    - Number of accedents by 71%.
    - Number of Deaths by 60%
    - Number of Injaries by 45%.
