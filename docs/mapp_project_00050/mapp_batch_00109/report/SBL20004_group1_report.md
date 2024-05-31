# Metabolomics analysis report
SBL.20004

31.05.2024
___
Group A
-	Justine Genet
-	Etienne Diethelm
___
## Introduction
In their natural habitats, plants are the target of a large number of herbivores, particularly insects and their larvae. They therefore need to protect themselves, and one way of doing this is through the production of secondary metabolites. The main classes of secondary metabolites involved in defense against herbivores are terpenes, phenolic compounds and nitrogen-containing secondary products such as alkaloids and glucosinolates.

The aim of these project was to try to detect those defense compounds by analysing the change in the metabolome of _Biscutella laevigata_ in response to herbivory by _Plutella xylostella_. 

_Biscutella laevigata_, the buckler-mustard, is a plant from the _Brassicaceae_ family, growing in the alpine regions of Europe. _Plutella xylostella_ , the diamondback moth, is a moth species from the Plutellidae family. The larvae feed on the plants of the _Brassicaeae_ family. 

## Material & Methods
### Experimental setup
The plants were grown from seeds in greenhouse condition at the University of Fribourg. The herbivores were obtained from Syngenta and reared in growth chambers.
The treatment consisted of approximately 20 larvae put on one leaf for 24 hours. 3 plants were treated and 3 others served as control. 

### Sample collection
One leaf was collected per control plant. On the treated plants, the leaf that received the herbivores were collected, as well as an other leaf on the same plant for the 'distant treatment'. The larvae that fed on the leaves were also collected for analysis, as well as larvae that didn't came in contact with the plants as control.
After collection, each sample was immediately frozen in liquid nitrogen in order to stop any metabolic reaction.

•	Link to the iNaturalist entries of your species.
### Sample preparation

Each sample were dry and then weighted, and put in centrifuge tubes. To extract metabolites, 1700µl of a solution containing 80% of methanol, 20% of H2O and 0.1% of formic acid  were added. Tubes were put in Mixer Mill, disrupt the tissues. Then, the samples were prepared for the MS. In addition to the prepared samples, we also mixed the plants into a new sample, and a second one containing the plants and the herbivores, as quality controls.
### LCMS Analysis
The LC conditions were describe [here](https://github.com/commons-teaching/SBL.20004.2024/blob/main/lc_conditions.txt) and the MS conditions [here](https://github.com/commons-teaching/SBL.20004.2024/blob/main/ms_conditions.txt).

### Data treatment
Those software were used : 
* MzMine, to filter the results of the MS and features related.
* Sirius, to identify the different compounds present in our samples.
* GNPS, which allow the connection of the different features analyzed, related to one compound. 
* Cytoscape, which permit the visualization of the molecular network between the different compounds and their features.

## Results
### MS1
After filtering with MzMine, the amount of features could be reduced to 4436.  The feature list can be found [here](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/results/mzmine/mapp_batch_00109_quant.csv)

### Molecular Network
Figure XXX show the molecular network of our features. Each node is represented by a pie chart, whose size is proportionate to the peak area of the feature. The colors indicate from witch samples the feature come, blue being control plant, pink distant treatment on plant, red direct treatment on plant, orange control larvae and yellow treatment larvae.
## Conclusion
Some conclusion that you could get out of this preliminary study.
