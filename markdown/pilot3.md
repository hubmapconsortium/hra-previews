#  Preview: HRA vs. Experimental Data

HuBMAP Atlas Previews demonstrate functionality and resources that will become available in future releases. Previews may rely on externally hosted data or analysis results that were generated with processing pipelines that are not yet integrated into the HuBMAP Data Portal infrastructure.


### Description

The “[An atlas of healthy and injured cell states and niches in the human kidney](https://www.biorxiv.org/content/10.1101/2021.07.28.454201v1)”, uses Human Biomolecular Atlas Program (HuBMAP) and the Kidney Precision Medicine Project (KPMP) data to create a high quality kidney atlas. The 21 tissue blocks used in the paper contain 64,693 kidney nuclei (10x Genomics snRNA-seq) from healthy reference states across 13 patient donors. Samples were derived from nephrectomy, biopsy, or deceased donor tissue, spanning three anatomical regions: medulla, cortex and papilla. See information on [kidney Azimuth reference](https://azimuth.hubmapconsortium.org/references/#Human%20-%20Kidney). 

The kidney Azimuth reference was cross-walked to the kidney ASCT+B table using this manually compiled [lookup table](https://github.com/hubmapconsortium/azimuth-annotate/blob/main/data/kidney.json). The result is an “augmented kidney ASCT+B table” with information on the number of cells per cell type (percentage per total can be computed from that).  

Out of the 21 tissue blocks, 18 could be registered using the [Registration User Interface (RUI)](https://hubmapconsortium.github.io/ccf-ui/rui); for the other three, no data exists for their source location. For the 18 registered blocks, ccf_annotations exist that identify the AS in the 3D kidney reference organ that collide with the tissue blocks. Using the ccf_annotations in combination with the “augmented kidney ASCT+B table” it is possible to identify/predict the number of cells per cell type associated with each tissue block.   

The below bar graph visualization shows cell type populations (pick counts or percentages) for the Azimuth and HRA bars on left and the 21 tissue blocks on right. The 21 tissue blocks can be grouped by sex, ethnicity, location or laterality.    

As atlas quality and coverage increase, atlas predictions will align with tissue sample cell type populations--for tissue blocks collected from comparable demographics. As tissue mapping protocols advance, tissue blocks collected from comparable demographics will show similar cell type populations. Note that the data collected for the kidney atlas paper purposefully covers tissue from different demographics. 

### Atlas Details

Azimuth is a web application that uses an annotated reference dataset to automate the processing, analysis, and interpretation of a new single-cell RNA-seq experiment. Azimuth leverages a 'reference-based mapping' pipeline that inputs a counts matrix of gene expression in single cells, and performs normalization, visualization, cell annotation, and differential expression (biomarker discovery). All results can be explored within the app, and easily downloaded for additional downstream analysis.  

The Human Reference Atlas (HRA) aims to map all of the cells of the human body to advance biomedical research and clinical practice. Please see [Perspective paper](https://www.nature.com/articles/s41556-021-00788-6) that presents collaborative work by members of 16 international consortia on two essential and interlinked parts of the HRA: (1) three-dimensional representations of anatomy that are linked to (2) tables that name and interlink major anatomical structures, cell types, plus biomarkers (ASCT+B). The paper also discusses four examples that demonstrate the practical utility of the HRA.   

### Experimental Data Details

Experimental data reported here is detailed in the paper “[An atlas of healthy and injured cell states and niches in the human kidney](https://www.biorxiv.org/content/10.1101/2021.07.28.454201v1)”. 

### Contributors

**Kidney Data:** [Authors](https://www.biorxiv.org/content/10.1101/2021.07.28.454201v1)

**Azimuth Kidney Reference:** Rahul Satija & KPMP Team 

**ASCT+B Kidney Master Table:** 
* Authors: Sanjay Jain, M. Todd Valerius, Yongqun He. 
* Reviewers: Blue Lake, Becky Steck, Rachel Dull, Ellen M. Quardokus. 
* [Master Table](https://hubmapconsortium.github.io/ccf-releases/v1.1/docs/asct-b/kidney.html)

**HRA vs. Experimental Data Bar Graph Visualization:** Amber Ramesh, Bruce W Herr II, Katy Börner


### Attribution

| Group  | Creater(Blue Lake & Sanjay Jain) |
|--------|----------------------------------|
| RTI-GE | Fiona Ginty (fiona.ginty@ge.com) |
| MC-IU  | Katy Börner (katy@indiana.edu)   |


### Visualization

<div class="video-container">
    <a target="_blank" href="https://hubmapconsortium.github.io/tissue-bar-graphs/preview" >
        <img src="../img/pilot3.png" height="550">
            </img>
    </a>
    
</div>

Sort the tissue bar graph by **sex** to see the results.

Open the visualization in <a target="_blank" href="https://hubmapconsortium.github.io/tissue-bar-graphs/preview" >new window.</a>

