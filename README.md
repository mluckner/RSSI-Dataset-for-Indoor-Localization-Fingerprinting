# RSSI-Dataset-for-Indoor-Localization-Fingerprinting
RSSI dataset collected in LOKKOM project

The data set contains coherent data collected in various buildings using the same methodology in three different buildings 
belonging to Warsaw University of Technology: Faculty of Mathematics and Information Science (*mini*), Faculty of Physics (*gf*) 
and Main building of Warsaw University of Technology (*gg*).

The data were collected in two independent and separated series between 07.2014 and 10.2014. The previous series was used as the learning set. 
The later series created the testing set. The location fingerprints in each of the two series create mostly a $1.5\times 1.5$ m grid. 
The grid was sparser when it was forced by the building's structure—walls or different obstacles. 
Both series cover the same building area and the corresponding points from the learning and testing series are shifted by 0.75 m 
in each direction to avoid an intersection. 

The data were collected using the Android application created for the LOKKOM project https://www.researchgate.net/project/LOKKOM
and operated on three different models of mobile phones with Android OS 2.1: HTC One, LG Nexus4, and Sony Xperia.
During the measurements, the phones were transported and rotated on a trolley. The measurements have been done in four directions parallel 
to the building axes. Its purpose is to consider the power absorption of the human body (operator). 
Therefore, there were 40 fingerprints taken at every measurement point, ten in each direction. 

 ## Publication
 
M. Luckner, S. Sowik and P. Brida, "Selection of Signal Sources Influence at Indoor Positioning System," in IEEE Transactions on Wireless Communications, vol. 23, no. 1, pp. 45-57, Jan. 2024, doi: 10.1109/TWC.2023.3275537. 
 
 ## Dataset
The RSSI dataset contains a folder for each building (*mini*, *gf*, *gg*). The complete data from the building are stored as an archive zip file. Additionally, a sample collected in a single POI (40 records) is given.

### Structure
- *building* building ID (*mini*, *gf*, *gg*)
- *series* series ID (1 - learning series, 3 - testing series) 
- *poi*	 measurement point ID
- *x* x coordinate of the measurement point
- *y*	y coordinate of the measurement point
- *z*	z coordinate of the measurement point
- *floor* floor of the measurement point
- *tick* the number of measurement in the reference point
- *direction* orientation of the measurement device according to the building axis (0-3)
- *timestamp* timestamp of the measurement
- *AP_i* reading from the ith access points (NA for lack of signal)

## Acknowledgement
The LOKKOM project was supported by the National Centre for Research and Development, grant No PBS2/B3/24/2014, application No 208921.
