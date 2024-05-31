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

_Biscutella laevigata_, the buckler-mustard, is a plant from the _Brassicaceae_ family, growing in the alpine regions of Europe. _Plutella xylostella_ , the diamondback moth, is a worldwide spread moth species from the Plutellidae family. The larvae feed on the plants of the _Brassicaeae_ family. 

## Material & Methods
### Experimental setup
The plants were grown from seeds in greenhouse condition at the University of Fribourg. The herbivores were obtained from Syngenta and reared in growth chambers.
The treatment consisted of approximately 20 larvae put on one leaf for 24 hours. 3 plants were treated and 3 others served as control. 

### Sample collection
One leaf was collected per control plant. On the treated plants, the leaf that received the herbivores were collected, as well as an other leaf on the same plant for the 'distant treatment'. The larvae that fed on the leaves were also collected for analysis, as well as larvae that didn't came in contact with the plants as control.
After collection, each sample was immediately frozen in liquid nitrogen in order to stop any metabolic reaction.

[Here](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/report/observations-440472.csv) you can find the link to the iNaturalist entries of the species.
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
After filtering with MzMine, the amount of features could be reduced to 4436.  The feature list can be found [here](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/results/mzmine/mapp_batch_00109_quant.csv).

### Statistical analyses
Statistical analyses were performed by the supervisor. On figure 1 you can find a heatmap of the significant features present in the plant samples. You can clearly see that the componds produced by the control plants (pink) are different that from the directy treated plants (red). The indirecty treated plants show similar pattern as the control for circa half of the componds, and similar to the directly treated for the second half. 

![heatmap](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/report/pictures/heatmap.png)
![heatmap legend](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/report/pictures/heatmap_legend.png)
> Figure 1: Heatmap of the significant features present in the plant samples.

Figure 2 is a treemap chart of the class of compond that was identified. In yellow are the feature that are found more in the treated plants, and in gray the ones that are more present in the controls
![treemap](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/report/pictures/treemap.png)
> Figure 2: A treemap of the metabolomic variation of _Biscutella laevigata_ whith and without herbivory.


### Molecular Network
Figure 3 show the molecular network of our features. Each node is represented by a pie chart, whose size is proportionate to the peak area of the feature. The colors indicate from witch samples the feature come, blue being control plant, pink distant treatment on plant, red direct treatment on plant, orange control larvae and yellow treatment larvae.
![molecular network](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/report/pictures/molecular_network.png)
> Figure 3: a picture of the molecular network. Blue = plant control, purple = plant distant treatment, red = plant direct treatment, orange = herbivor control, yellow = herbivor treatment
#### Examples of compounds of interest
On the molocular network, we can find some promising compounds, that seem to be produced in higher amount in the plant under herbivory attack than in the control plant. Many of these are alkaloids and compounds containing sulfur, known for their role in defending plants against herbivores. 
Figure 4 show an isothiocyanate. Isothiocyanates are often product of metabolic conversion of glucosinolates. It suggest a compond involved in plant defense.
![577](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/report/pictures/577.png)
> Figure 4: Feature n°577, an isothiocyanate

On figure 5, you can appreciate the molecular network of an alkaloid. Alcaloids are among the most important metabolites in the defense of plants against their natural enemies.
![1774](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/report/pictures/1774.png)
> Figure 5: feature 1774, an alcaloid

On figure 6, you can find a sulfoxide, a sulfure containing compond.
![383](https://github.com/commons-teaching/SBL.20004.2024/blob/main/docs/mapp_project_00050/mapp_batch_00109/report/pictures/383.png)
> Figure 6: feature 383, a sulfoxyde.



## Conclusion
Despite the gigantic amount of data produced by the LCMS method, some limitations persist, making it difficult to interpret the results.

Firstly, no feature was at the same time statistically significant and making sense on the molecular network. For example there should be a significant difference in the control and treated plant and being absent from the blank or the herbivore. Feature that are isolated and not taking part in a network are also suspicious. To solve this problem, a larger number of replicates would have been needed, in order to see statistically more robust results.

Secondly, most of the feature could not be identified precisely. And even when we were able to obtain a molecule name, there was almost no literature about it, at least in plant biology. It is therefore impossible to provide an interpretation without literature to refer to.

However, since the aim of this project was to highlight a change in the Biscutella metabolome in response to herbivory, we can consider that this goal has been achieved. 
