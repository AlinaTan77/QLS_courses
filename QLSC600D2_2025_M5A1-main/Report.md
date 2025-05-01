---
output:
  pdf_document: default
  html_document: default
---
# Reproducibility of Papers on Different Fields

## Notes

## Microbiology

## Paper 1: Cartography of opportunistic pathogens and antibiotic resistance genes in a tertiary hospital environment (2020)

### Data availability and accessibility
The paper was published under open-access. The original fastq sequencing data (as well as SRA and BAM files) have been made available through an accessible online database (Project PRJEB31632) in the European Nucleotide Archive with a link to the database page embedded within the published paper. A significant amount of supplementary data (e.g. metadata, taxonomic and resistome profiles, patient isolates) that was not published in the main article are also available; this supplementary data was also analyzed and 13 supplementary figures and 3 notes are provided to readers as a part of the publication (via free download from the Nature Medicine website). 

### Quality of experimental design	
This particular research is an observational study with spatio-temporal specificity. Therefore, certain criteria such as blinding and randomization of samples were not appropriate for this particular work. Technical replicates were not performed for environmental sampling nor culture enrichment of swabbed samples. Controls, spike-ins, and validation experiments were performed for kit (i.e. reagents and DNA extraction kits, etc.) contamination effect on environmental samples, particularly low biomass samples. Negative control swabs were performed to monitor swab contamination. Data exclusions were clearly acknowledged (e.g. samples with low DNA yield below sequencing threshold) and the number of total exclusions (3 out of 358 DNA libraries) were provided by the authors. For significant results discussed in the paper, the type of statistical analysis, resulting P-values, and accompanying assumptions were provided within the results. The paper is also accompanied by a "Reporting Summary" which Nature Research implemented to improve reproducibility and transparency in their published works. This Reporting Summary very clearly outlines the life sciences study design and makes it easy for the reader to understand the design limitations and reasons why a design method was selected for the undertaken research. No conflicts of interest were noted.

### Description of methods	
The methods are detailed and quite lengthy; therefore, seemingly to maintain clarity, the methods section was published at the end of the publication following the references section. Additionally, the references cited within the methods section were listed inside the methods section in a type of sub-references section. This also improved clarity as it helps with  cross-referencing papers used in the method development. The paper concludes that culture enrichment of low-abundance resistant pathogens combined with long read sequencing is powerful and suitable for recovering genomes without isolation. Although a very exciting work, the paper does not describe if "laboratory artifacts" are introduced to bacteria-of-interest during the enrichment step: the facilitation of bacterial conjugation to exchange resistance-encoding genes could be problematic to the concluding results if true. 

### Description of sample population/data under study	
Due to the observational nature of this study (i.e. antimicrobial resistance surveillance study), the sampling population is limited to various locations within one tertiary hospital in Singapore. Bias of sample selection (whether environmental or clinical) could arise due to this inherent limitation in sampling large areas under study. This paper also uses previous data collected using different methods performed over a decade ago. Interestingly, using these two data sets, they found five nearly identical strains of Staphylococcus aureus persisting in the same hospital environment for over 8 years at the time of the research work. However, it is unclear if these strains were stable for the entire duration or were reintroduced at some point.

### Tool accessibility 
All software used and their respective versions used are explained in detail. The statistical analyses were "performed in R" but no packages were described (if used). The equipment and reagents used were also described in detail in the methods section and their respective commercial sources were also listed. 

## Paper 2: Linking the resistome and plasmidome to the microbiome (2019)

### Data availability and accessibility
The paper was originally published in 2019, and its publishing journal became fully open access on January 1st 2024. The original fastq sequencing data are available through an accessible online database (Project PRJNA50646) in the Sequence Read Archive data repository. Supplementary data and code for analyses that was not published in the main article are also available through OSF Home, a free open platform for data sharing, and which was provided by the private research partner. 

### Quality of experimental design	
It is unclear how many replicates of the sequence libraries were made: the study describes taking a single wastewater sample at one time point and splitting it into sub-samples but does not elaborate. A single positive control of known bacteria with a sequenced plasmid was spiked to a subset of the environmental wastewater sample to maintain a known 10% concentration. The study concludes that spurious links found in the bioinformatics analysis were probably related to the high abundance of this spiked organism, resulting in some clusters relating to other organisms that were not expected to have had any relation to the plasmid. No follow-up or additional evidence as to why this was observed or if this was a statistically significant conclusion was provided. No discussion of the type of statistical analyses on the environmental sampling data were performed; statistical assumptions or significance statistics were not provided. Additionally, there are some methods that could be written in more detail, for example, it is unknown if cell pellets isolated from wastewater were frozen at -20 degrees Celsius in a storage buffer (e.g. glycerol solution), water, or just as a dry pellet: in this case, storage of unprotected cell pellets can be significantly damaged by freeze-thaw during sample processing and could impact inference of the data. Data exclusions were recognized and acknowledged, and reasons why provided; the authors discarded all contigs less than 1000 base pairs in size or which contained fewer than two restriction enzyme sites contig-cluster linkages represented by only one or two reads. Conflicts of interest were acknowledged in the paper: three of the authors are employees and shareholders of Phase Genomics, and two of these three are also executives of the company. 

### Description of methods	
The methods section fails to accurately describe the proximity ligation step of the protocol; the authors did not describe the DNA binding step (e.g. using formaldehyde) prior to cell lysis within the article body; the authors did refer to the use of the commercial ProxiMeta Hi-C Preparation Kit by Phase Genomics to create the Hi-C library but further inspection of the Hi-C Preparation Kit protocol (which was not linked to in the article) has the reagents listed with generic names (e.g. Crosslinking buffer) rather than chemical names and their respective components. The authors did include Figure 1a which depicts this covalent bonding step (via formaldehyde), although prior to the Hi-C library construction, though this is not clearly described in the methods section. Inadvertently, this could be very confusing for readers not familiar with the covalent binding step of cell nucleic acids for proximity ligation. Additionally, the flow cytometry protocol for environmental cell counts was not described.

### Description of sample population/data under study	
The title of the paper, "Linking the resistome and plasmidome to the microbiome"" is too generic and could be misconstrued as misleading. For this paper, the title should allude to the fact that only one wastewater sample was taken at a single time point in October 2017, and then split into fractions (in which only one was spiked) and analyzed. The extrapolation of this small sample set to any other environmental, clinical, human, or animal microbiome environment is far-reaching at best. There is no provided metadeta of the wastewater sample (e.g. pH, total and volatile solids content, chemical oxygen demand, fecal coliform concentrations, ammonia/ammonium, organic acids, etc.) which greatly impact not only microbial cells and their growth but also downstream processing. This paper is at its heart a methodological validation experiment, and therefore the poor characterization of samples is exasperating. 

### Tool accessibility 
Software used was provided, though exact versions used were not always described. Analyses of the Hi-C libraries were performed using a proprietary pipeline developed by the private research partner and was acknowledged in the paper. Not all of the equipment and reagents used were described in enough detail in the methods section, for example, the make and model of the flow cytometer used for cell counts was not described nor the "R2A agar" media for colony forming unit (CFU) counts was not provided with a recipe list nor the commercial vendor (if applicable). 

## Genetics
## Paper 1(AT): Human genetics evidence supports two-thirds of the 2021 FDA-approved drugs (2022)
### Data availability and accessibility
The paper was originally published in Nature Reviews Drug Discovery under the biobusiness briefs section. The codes are accessible, with the link provided in the article. However, the platform used to store their data is unavailable.

### Quality of experimental design	
The study aims to find genetic support for FDA-approved drugs. For the experimental design, it utilized 15 different databases to identify evidence.

### Description of methods	
The methods are explained in the supplementary documents. Initially, Drug IDs were converted to Gene IDs, followed by leveraging 15 different genetic resources as integrated by the Open Targets Platform. Related traits to the drug indication were manually included, with the availability of genetic evidence for the drug target.

### Description of sample population/data under study	
They used 15 different genetic resources, which is very comprehensive and covers a wide range.

### Tool accessibility 
The code and data are available online, but the software used to store their data, known as "spark," is not accessible without Google Cloud storage, which requires payment.

## Paper 2(AT): An effector index to predict target genes at GWAS loci (2021)
### Data availability and accessibility
The paper discusses the development of the effector index, utilizing GWAS summary statistics or individual-level genetic data. All data and code mentioned in the original paper are accessible online, although the data preprocessing and evaluation codes used is not provided. Positive control genes for evaluation were sourced from databases such as the Human Disease Ontology database, OMIM linkage information, and a study by Morris et al. Additionally, GWAS summary statistics were gathered from various publicly available resources and through GWAS conducted on UK Biobank traits. The paper thoroughly identifies all other data sources utilized in the study.

### Quality of experimental design	
The experimental design is clearly delineated, with each step thoroughly explained. Hyperparameters in XGBoost, such as tree depth, lambda, and gamma, were fine tuned to optimize cross-validated performance on training data. Performance evaluation was conducted using the area under both receiver operating characteristic curves (AUC-ROC) and precision-recall curves (AUC-PRC) on test datasets, ensuring comprehensive assessment of model effectiveness.

### Description of methods	
They provided a detailed flowchart of the method, which begins with fine-mapping of GWAS summary statistics, followed by annotation of single nucleotide variants (SNVs) to identify potential causal variants and their association with genes within or near the GWAS loci. Subsequently, these data are leveraged to generate gene- and locus-level features, integrating information on the presence of specific SNVs within genes, their functional implications, and locus-specific characteristics. Feature weights within the models are determined through leave-one-out analysis, facilitating the assessment of model robustness and generalizability. The performance of the models is then evaluated by predicting target genes for loci containing positive control genes, with comparisons made to known positive control genes. This evaluation aims to measure the model's accuracy in identifying true target genes while minimizing false positives and false negatives, thus providing insights into its effectiveness in prioritizing genes at GWAS loci.

### Description of sample population/data under study	
The data utilized in the study consists of GWAS data associated with 12 common traits. These traits include Type 2 diabetes, estimated bone mineral density, diastolic blood pressure, height, hypothyroidism, red blood cell count, systolic blood pressure, calcium, direct bilirubin, glucose, low-density lipoprotein, and triglycerides. This diverse range of phenotypes or conditions provides a comprehensive dataset for the analysis and development of the effector index discussed in the study.

### Tool accessibility 
The tools required for the study are publicly available, although the algorithm is implemented in a mixture of Shell and R. Despite their availability, the absence of a guideline or readme file may pose challenges in utilizing these tools effectively. This lack of documentation could potentially hinder users' ability to understand and apply the algorithm, thus reducing its accessibility and usability. 

### Replicability 
The algorithm utilized in the study can be replicated for use with GWAS data associated with different traits. However, replicating the data preprocessing steps may present challenges as the code for this process is not provided. Lack of access to the preprocessing code could hinder the replicability of the study, as it may be difficult for other researchers to precisely reproduce the initial data preparation steps. Providing the preprocessing code or detailed instructions would enhance the replicability of the study and facilitate its adoption by other researchers interested in utilizing similar GWAS datasets.

## Molecular Biology

## Paper 1 (LH): Single-molecule tracking reveals the functional allocation, in vivo interactions, and spatial organization of universal transcription factor NusG (2024)

### Data availability and accesibility
This paper is published under open access through Cell Press Journals. A key resource table is provided which lists all reagents, bacteria strains, data and software etc., their source and identifier (if applicable). Fluorescence imaging dataset is published and openly available on Mendeley. Links are provided to the sources of the code and softwares used, however one of the softwares is reported to be no longer supported. Contact information is provided for the lead author along with a statement acknowledging information will be provided upon request if needed to reanalyze the data. A statement is provided acknoledging that all strains generated in the study will be provided upon request. All this information was provided in a section called STAR Methods. STAR stands for Structured, Transparent, Accessible Reporting. This is a methods format introduced in 2016 that has been adopted by all Cell Press journals (https://www.cell.com/star-authors-guide).

### Quality of experimental design
- Sequencing was performed on the constructs as validation
- Bootstrapping analysis is performed to calculate fitting errors for the D* distributions
- In the methods there is a statement claiming experimental repeats were performed for each condition to define the reproducibility of the results however I don't see anywhere in the paper where this reproducibility is quantified.
- Many conditions were tested to solidify their conlcusions regarding the different NusG populations and their corresponding functions/interactions. For each of these conditions a similar number of NusG molecules were observed (order of 10 000), maintaining similar statistical power for each measurement. For example, when characterizing the fast population, three different conditions were measured improving the robustness of their conclusions (as oppose to making a conclusion from one condition).

### Description of methods
- There is a clear, specific description of the methods used to create each new bacterial strain. For construction procedures that are well known, references are provided to early papers that give in depth details of the procedure. A supplemental table is also provided outlining the names of each strain, their use for the paper and their genotype.
- The methods described for immunoblotting contained specific details regarding temperatures, times, volumes, and reagents. I have not performed immunoblotting but I feel that the methods described here are specific enough that I would be confident with replicating the procedure.
- Cell preparation methods go into very specific details, explicitly stating all variables invovled in this process
- For single molecule imaging, the various parts of the custom built microscope (lasers, camera, objectives, modulators, etc.) were explicitly stated along with their respective provider and identifying code. Additionally the acquisition details were provided.
- SIM imaging acquisition details were described in depth. Additionally, references are provided directing to papers with further details on the 3D imaging procedure.
- For single molecule tracking analysis a reference is provided to a previous paper where the same method was used. A brief description is also provided, while the methods in the previous paper are in great depth.

### Description of sample population/data under study	
This study is examining the dynamics of NusG (a molecule) in E. coli to make inferences about the different NusG populations and their abundance. One could thus claim that the sample population is the NusG molecules. For each distribution that was reported the number of NusG molecules contributing to the distribution was reported in the figure caption which averaged around 40 000. These molecules were sampled from many E. coli cells (order of hundreds) in multiple fields of view (not specified numerically). For this type of study, I would claim that the sample population is representative (not just collected from one experiment/ one field of view / one cell). One improvement would be including the number of fields of view and experimental repeats with the statement made in the Quantification and Statistical Analysis statement. 

### Tool accessibility
- The microscope used for single-molecule tracking PALM is custom built, thus it is not easily accessible unless you are located at their institution (Oxford). A detailed description regarding the microscopes specs was provided which allows people to identify a commercial microscope that is comparable.
- The microscope used for SIM imaging is commercial - more accessible than custom built
- Single molecule localizations performed with custom software
- As previously stated, links are provided for open access code and software that were used for analysis.

## Paper 2 (LH): Single molecule microscopy reveals key physical features of repair foci in living cells (2021)

### Data availability and accesibility
This paper is published by eLife which is an open access journal. All single molecule imaging files are made available on zendo and the link provided is functional. This data availability should be sufficient to attempt replication of the analysis reported in this study. Additionally, detailed tables outlining the yeast strains and the primer sequences used in the study are provided.

### Quality of experimental design
This paper is performing single molecule tracking of a DNA repair protein in yeast. The sample sizes used in analysis seem reasonable (many different cells and many traces per cell). The choice of model used to fit the data is well informed (statistical tests performed to compare different models). Validation experiments were performed to assess the impact of adding a fluorescent tag to the protein had on cell functionality. Multiple condtions were studied (no DNA breaks vs double stranded break, compare dynamics to single stranded DNA binding protein, comparison with mobility in diploid cells) which are logical and inform the conclusions. 

### Description of methods
Overall, the methodology section is very thorough and includes specific details such as temperatures, concentrations, protocol times, and image acquisition  details that are necessary to reproduce the experiments. Where further details could be needed include, a description of the parameters used to tracking single molecules and a description of the algorithms used for the simulations. For most protocols described in the methods a link is provided to bio-protocol where one can request more details. This is described to be part of eLife's effort to make science more reproducible and may not necessarily be a reflection of the author's willingness to respond.

### Description of sample population/data under study
A table of all yeast strains used in the study is provided which includes their genotype and origin. It is reported that for each condition, at least 3 independent experiments were performed using different samples prepared from different colonies. The study also specifies that all cells were chosen at the same cell cycle phase and their method of identifying it. In the supplementary material, a table is provided that lists for a particular condition, the number of cells, single molecule traces, and single molecule displacements that contributed to the analysis. This is a clean way of communicating the sample sizes to the reader. The table is however, provided as a .tex file whereas a pdf file could have easily been used instead that would be more accessible to a general audience. 

### Tool accessibility
All microscopy was done on a custom set-up, however, they name a commericial microscope that it is based on which would is likely easier to access. All code used in the analysis is custom and not shared. Very little information is provided about the analysis code (no reference to language or software) making it challenging to perform an exact replication of the analysis.

### Additional notes
eLife includes a transparent reporting form with the publication where the authors are asked to comment on sample-size estimation, replicates, statistical reporting, group allocation, and additional data files. The authors provided reasonable responses to each section. 

## Computer Vision
## Paper 11: Organizing principles of astrocytic nanoarchitecture in the mouse cerebral cortex (2023)

### Data availability and accesibility
Data appears to be available and accessible. However, it is stated that all data reported in the paper can only be accessed upon request to the lead contact, who is the principal investigator of the lab which produced the article. Although lead contact information is provided, the response and delivery time will most likely vary and is dependent solely on the lead contact. Perhaps creating a webpage with downloadable links would resolve this concern by eliminating the need to first reach out to the lead contact.

### Quality of experimental design
Overall, the quality of the experimental design is simple yet complex. Given that the goal was to resolve astrocytic architecture, the authors wisely used imaging techiniques that yielded the highest resolution possible, focused ion beam scanning electron microscopy. With this approach and manual segmentation labour, the researchers were able to yield a detailed 3D reconstruction of astrocytes and certain physical features. In addition, the researchers reported ample quality control of the manual segmentation. The researchers were aware about the issues that may arise due to the nature of hand segmentation and made efforts to minimize error. In order to analyze the segmentation data, the researchers applied suitable algorithms for the 3D space the data resided in. There appeared to be a clear reasoning for the selection of each algorithm to yield answers to each astrocytic architecture question asked.

### Description of methods
The methodology section of this article was certainly extensive and clearly organized. The authors subdivided this section logically into partitions such as tissue preparation for light microscopy, focused ion beam scanning electron microscopy, and 3D reconstruction. Quantification and statistical analysis was its own section that immediately followed. In total, there were 13 methodology subcategories with not a single detail appearing to be missed. The amount of information covered, although vast, was made digestible by the subsectioning and the chronological ordering.  

### Description of sample population/data under study	
The data analyzed was gathered from mice brain tissue and the researchers provided a sufficient amount detail about the organism strains. In addition to strain information, the authors also included a great amount of detail regarding the tissue collection procedure from the purchasing of the mice to the brain removal surgery.

### Tool accessibility
All resources and tools are accessible. This is shown through the article's clear and extensive key resources table which included information regarding all resource categories such as chemicals, organisms, and software. The table was well organized such that for each resource, there included its name, source company, and identification code. Having data information presented in the elegant table manner makes it easy for readers to obtain the exact same resources if needed. All code used in the article is neatly organized on a GitHub repository with clear instructions and sample data to operate on. One concern is the sheer man power and time needed to perform this experiment specifically for the segmentation stage. 

## Neuroscience
## Paper 12: Glycogen distribution in mouse hippocampus (2019)

### Data availability and accesibility
There appears to be zero effort made by the authors to make the data included in this article available or accessible.

### Quality of experimental design
The researchers make the point that their glycogen analysis methodology is an improvement on those that have been used in past studies. In previous studies, researchers have used the periodic acid-Schiff staining method to visualize glycogen levels. This method is not glycogen specific but rather stains for glycoproteins and proteoglycans. Another downfall of past studies that during the collection of brain tissue, glycogen is depleted during one of the necessary steps for immunohistochemistry and consequently invalidates the evaluation of glycogen concentration and distribution. To combat these known flaws of glycogen analysis, the researchers made the careful decision to use an antibody that is specific to glycogen and use a technique called focused microwave irradiation which preserves the state of glycogen at the time of collection by inactivating enzymatic activites. To provide evidence of how the methodology of the current paper is superior to past studies, the authors included figures clearly demonstrating the glycogen specificity of the antibodies and the glycogen preservation of the microwave fixation procedure.
In terms of investigating the immunohistochemistry results, all observations were qualitative and lack statistical analysis. Observed patterns such as certain hippocampal layers being more rich in glycogen are accompanied by unanswered questions such as how were layer boundaries defined? How were glycogen concentration levels determined? Although the role of this paper may have been to provide solely qualitative observations, basic explanations as to how these qualitative observations were obtained should have been included.

### Description of methods
Overall, the methodology of this paper is weak. In fact, there was no section dedicated to the methods. Details are dispersed and intertwined with background information. This poor organization provides the reader with the inconvenient task to parse through the entire paper to filter for methodology components. Before discussing the methodology for the first time, the authors state that they will "summarize" the histological procedure. This statement seems to assert that the researchers were fully aware about how much detail was going to be omitted in this article. The researchers provide rudimentary information regarding the collection and preparation of the brain tissue for light microscopy such as how the brain tissue was removed and fixed, which antibodies were used, and what they stain for. The authors ask the reader to refer to another paper for all immunohistological procedure details. In terms of their qualitative observations, no details as to how they came to these conclusions are listed. All statements about glycogen distribution appear to be made by visual judgement. 

### Description of sample population/data under study	
In the article, no information is directly given about the mice strain. Mice information can be found in a separate paper the authors reference. It would have been helpful to include basic information about the organism and its tissue in the present article.

### Tool accessibility
Light microscopy equipment is usually easily accessible. However, the microwave fixation system is most likely a limiting factor. The present paper and other papers who used the system all did so in Tokyo, Japan at a specific company. In addition, purchasing information is not readily available on the company's website.


## Computational Neuroscience
## Paper 1 (RFJ): Go with the FLOW: visualizing spatiotemporal dynamics in optical widefield calcium imaging (2021)

### Data availability and accesibility
All data and code presented in this paper are publicly available (open access). You can access the data and code repository at the following link: https://royalsocietypublishing.org/doi/10.1098/rsif.2021.0523#d1e2672. The repository includes both the code used in the experiments and the associated data, encompassing both raw and processed datasets, all openly accessible.  Additionally, supplementary videos have been provided for result comparisons mentioned in the paper. Some of the data sources are referenced in another paper co-authored by one of the contributors to this study.

### Quality of experimental design
This paper relies on algorithmic outputs applied to available data for its results. The chosen sample size appears reasonable for conducting a statistical analysis; however, concerns arise regarding the statistical methods employed. Specifically, a pairwise t-test was conducted on the distribution of ridges derived from their code, yet the rationale for choosing this test method remains unclear. Notably, the t-test typically assumes normal distribution of data, a point unaddressed in their explanation.

Furthermore, the reported small p-value, emphasized as validating the assertion of changes in brain dynamics for older mouse pups, raises skepticism. It is unclear whether the small p-value results from the inherent minuteness of the effect or if it genuinely reflects statistical significance. Compounding this, the authors lack a substantial dataset for comparison, as evidenced by their use of mean values to calculate a p-value on the order of 10^(-4). These factors contribute to ongoing reservations about the robustness and generalizability of the statistical findings. 

### Description of methods

This paper primarily delves into the implementation of a specific algorithm applied to mouse brain datasets, with a notable emphasis on elucidating the underlying principles and mathematical theory governing the code's functionality. However, the conceptual explanation assumes a degree of familiarity with fluid dynamics, making it somewhat challenging for those without intensive training in the field.

Regarding the dataset, the authors provide references for additional insights into the mouse population details. The methods for the surgical procedures during widefield imaging are meticulously outlined, along with specific information on the employed calcium indicators. Despite these clarifications, certain steps, particularly those related to the type of brain activity analyzed in the mouse pup dataset, remain ambiguous. Additionally, the absence of a paper explicating the data gathering process for the mouse pup dataset raises questions.

Further, the rationale behind comparing specific age groups of mouse pups is not explicitly stated, leaving the reader with uncertainties about the significance of the chosen comparisons. Clarifying these aspects would enhance the overall comprehensibility and transparency of the study.


### Description of sample population/data under study

Two distinct categories of mice were involved in the analysis of their brain activity. The first group comprised mouse pups, with ages specified to be a maximum of 8 days postnatal, providing a comprehensive description of the age range for this subset. In contrast, the adult mouse dataset delineated both the age (approximately 30 weeks) and gender (male) in explicit detail within the paper.

### Tool accessibility
The code is released under the permissive license, granting users the freedom to use, modify, distribute, and sublicense with minimal restrictions. The code was sufficiently documented and seemed to be directly usable. Papers were also cited in order to understand further the underlying theory behind the algorithm constructed. 

## Paper 2 (RFJ): Optical-flow analysis toolbox for characterization of spatiotemporal dynamics in mesoscale optical imaging of brain activity (2017)

### Data availability and accesibility

In this paper, the authors utilized optical flow analysis tools and custom source and sink locators to investigate synthetic moving stimuli and mouse brain activity in the FLS1 and FLS2 regions. Supplementary videos demonstrating the application of these tools to the analyzed videos were provided alongside the paper. However, having access to raw data would be more useful in understanding the delta F/F calculation and its consequent effects. The accessibility of the raw data would enhance the transparency of the methodology, enabling a more thorough exploration of the analysis outcomes.

### Quality of experimental design

The study revolves around a MATLAB toolbox developed by the authors for extracting velocity vectors to analyze brain activity propagation on the cortex using optic flow. The paper concentrates on explaining the principles behind calculating time-varying velocity fields, their MATLAB implementation, and an assessment of the algorithm's performance.In the evaluation phase, the authors conducted a thorough comparison of velocity fields and angles, basing their analysis on theoretical parameters implemented in synthetic data. The assessment involved the application of the Horn-Shunck Algorithm, CLG method, and TS method. Despite featuring the CLG method, the authors candidly acknowledged its limitations within the analysis framework.The evaluation methodology displayed objectivity, encompassing a systematic comparison of the algorithm's performance against theoretical velocities. Notably, the authors measured the discrepancy between the toolbox-generated output and the theoretically expected velocities, contributing to a comprehensive assessment.The study's practicality was further demonstrated by testing the toolbox's resilience to noise inherent in widefield imaging data. Incorporating noisy data into the evaluation showcased the algorithm's robustness, adding a valuable dimension to its applicability in real-world scenarios.

### Description of methods

The explanation of the algorithms were thoroughly explained except for the TS method. It would be helpful, if not through mathematical equations, to use a figure to explain how the model works. Even though they provided the code and is sufficiently documented, the infographic of the TS Method workflow will still be helpful. 

The methods explained in finding sources and sink seemed to be very simple compared to what is written in the code. For example in finding the Poincare index, it was unclear the type of neighborhood they used in the calculation. There is also no understandable mathematical  equation that they showed regarding this. Therefore, it was difficult to understand. Furthermore, they did not explained why the usage of a 2x2 sub array is the most helpful method in finding the source and sink.

### Description of sample population/data under study

There were not much description regarding the mouse used for widefield imaging in this paper. I would understand why this is the case since their paper is only testing the toolbox to sample brain activity and synthetic datasets to demonstrate the effectiveness of their algorithm. The synthetic dataset that they use also captures the behavior of stimulus that are fundamental such as horizontal an radial propagation, source and sink simulation and shape translation.


### Tool accessibility
The authors have made their code openly accessible and distributed it, including the optic flow methods, and have even developed a user-friendly graphic interface named OFAMM for ease of use. While the methods for calculating sources and sinks lack explicit documentation, the provided steps on how to utilize the toolbox facilitate its application. However, there is a challenge in locating files generated by the toolbox, an aspect not addressed in the manual, which can pose difficulties for users navigating the output files. Clarity on file storage and retrieval would enhance the user experience, ensuring a smoother and more efficient utilization of the toolbox.

### Data availability and accessibility
All data and code presented in this paper are publicly available (open access). You can access the data and code repository at the following link: https://royalsocietypublishing.org/doi/10.1098/rsif.2021.0523#d1e2672. The repository includes both the code used in the experiments and the associated data, encompassing both raw and processed datasets, all openly accessible.  Additionally, supplementary videos have been provided for result comparisons mentioned in the paper. Some of the data sources are referenced in another paper co-authored by one of the contributors to this study.

### Quality of experimental design	

This paper relies on algorithmic outputs applied to available data for its results. The chosen sample size appears reasonable for conducting a statistical analysis; however, concerns arise regarding the statistical methods employed. Specifically, a pairwise t-test was conducted on the distribution of ridges derived from their code, yet the rationale for choosing this test method remains unclear. Notably, the t-test typically assumes normal distribution of data, a point unaddressed in their explanation.

Furthermore, the reported small p-value, emphasized as validating the assertion of changes in brain dynamics for older mouse pups, raises skepticism. It is unclear whether the small p-value results from the inherent minuteness of the effect or if it genuinely reflects statistical significance. Compounding this, the authors lack a substantial dataset for comparison, as evidenced by their use of mean values to calculate a p-value on the order of 10^(-4). These factors contribute to ongoing reservations about the robustness and generalizability of the statistical findings.  

### Description of methods	
This paper primarily delves into the implementation of a specific algorithm applied to mouse brain datasets, with emphasis on elucidating the underlying principles and mathematical theory governing the code's functionality. However, the conceptual explanation assumes a degree of familiarity with fluid dynamics, making it somewhat challenging for those without intensive training in the field.
Regarding the dataset, the authors provide references for additional insights into the mouse population details. The methods for the surgical procedures during widefield imaging are meticulously outlined, along with specific information on the employed calcium indicators. Despite these clarifications, certain steps, particularly those related to the type of brain activity analyzed in the mouse pup dataset, remain ambiguous. Additionally, the absence of a paper explicating the data gathering process for the mouse pup dataset raises questions.


### Description of sample population/data under study	

Two distinct categories of mice were involved in the analysis of their brain activity. The first group comprised mouse pups, with ages specified to be a maximum of 8 days postnatal, providing a comprehensive description of the age range for this subset. In contrast, the adult mouse dataset delineated both the age (approximately 30 weeks) and gender (male) in explicit detail within the paper.

### Tool accessibility 

The code is open acces and was released under the permissive license, granting users the freedom to use, modify, distribute, and sublicense with minimal restrictions. The code was sufficiently documented and seemed to be directly usable. Papers were also cited in order to understand further the underlying theory behind the algorithm constructed. 


## Paper 2 (RFJ): Optical-flow analysis toolbox for characterization of spatiotemporal dynamics in mesoscale optical imaging of brain activity (2017)

### Data availability and accessibility
The paper is easily accessible because it’s open access. In this paper, the authors used optical flow analysis tools and custom source and sink locators to investigate synthetic moving stimuli and mouse brain activity in the FLS1 and FLS2 regions. Supplementary videos showing the application of these tools to the analyzed videos were provided alongside the paper. While these videos offer practical insights, having access to raw data would be useful in comprehending the nuances of the delta F/F calculation and its consequent effects. The inclusion of raw data would enhance the transparency of the methodology, enabling a more thorough exploration of the analysis outcomes.

### Quality of experimental design	
The study revolves around a MATLAB toolbox developed by the authors for extracting velocity vectors to analyze brain activity propagation on the cortex using optic flow. The paper concentrates on elucidating the principles behind calculating time-varying velocity fields, their MATLAB implementation, and an assessment of the algorithm's performance. In the evaluation phase, the authors conducted a thorough comparison of velocity fields and angles, basing their analysis on theoretical parameters implemented in synthetic data. The assessment involved the application of the Horn-Shunck Algorithm, CLG method, and TS method. Despite featuring the CLG method, the authors candidly acknowledged its limitations within the analysis framework.
The evaluation methodology displayed objectivity, encompassing a systematic comparison of the algorithm's performance against theoretical velocities. Notably, the authors measured the discrepancy between the toolbox-generated output and the theoretically expected velocities, contributing to a comprehensive assessment. The study's practicality was further demonstrated by testing the toolbox's resilience to noise inherent in widefield imaging data. Incorporating noisy data into the evaluation showcased the algorithm's robustness, adding a valuable dimension to its applicability in real-world scenarios. 

### Description of methods	
The paper provides a comprehensive and detailed explanation of the algorithms employed, except for the TS method. The TS method was simply explained in the paper, however, it was not quite informative. While the code is available and well-documented, a visual representation of the TS Method workflow could serve as a valuable supplement, facilitating a clearer grasp of its functioning.
Concerning the methods for finding sources and sinks, the explanations appeared straightforward in the paper but seemed more complex in the code. For instance, the determination of the Poincare index lacked clarity regarding the type of neighborhood used in the calculation, and there was a noticeable absence of explicit mathematical equations. This omission made it challenging to fully comprehend the process. Additionally, the paper did not elaborate on why a 2x2 sub-array was chosen as the optimal method for identifying sources and sinks, leaving this aspect unclear.

### Description of sample population/data under study	

The paper notably lacks detailed descriptions of the mice used for widefield imaging, a gap that can be understood given the paper's primary focus on testing the toolbox for sampling brain activity and demonstrating the algorithm's effectiveness with synthetic datasets. The synthetic datasets employed in the study successfully capture fundamental stimulus behaviors, including horizontal and radial propagation, source and sink simulation, and shape translation. The emphasis on these synthetic datasets aligns with the paper's objectives, providing a controlled environment to showcase the toolbox's capabilities in handling various scenarios and validating its algorithmic performance. While the absence of detailed mouse descriptions may be justified in the context of the study's scope, future research or applications could benefit from incorporating additional details about the experimental subjects for a more comprehensive understanding of the study's context and potential real-world applications.

### Tool accessibility 

The authors have made their code openly accessible and distributed it, including the optic flow methods, and have even developed a user-friendly graphic interface named OFAMM for ease of use. While the methods for calculating sources and sinks lack explicit documentation, the provided steps on how to utilize the toolbox facilitate its application. The paths and names of saved files generated from the algorithm were also indicated for easier navigation through the outputs of the toolbox.

## Bioengineering
## Paper 15: Cancer Cell Membrane-Coated Nanoparticles for Anticancer Vaccination and Drug Delivery (2014)

### Data availability and accesibility
Data is, in theory, available upon request. Because the data set was produced in lab and the method is the most important aspect of this report, not big issue is put into making the data available directly without requesting it directly.

### Quality of experimental design
Design looks solid, because the study is mostly physical, we can see the the data analysis is just enough to show the trend is present.

### Description of methods
Method is the most solid aspect of this study, it goes very in depth into telling what each step is. Including the reagent concentration and device settings.

### Description of sample population/data under study	
Good description of the population. Almost N/A though since we are justlooking at the effect of the core composition in a medicinal setting.

### Tool accessibility
Other than the expensive equipment, the analysis software is fine

### Ophthalmology

## Paper 1 (RH): Coenzyme Q10 trapping in mitochondrial complex I underlies Leber’s hereditary optic neuropathy (2023)

### Data availability and accessibility
This paper is published under open access. It is a molecular dynamics simulation study of mitochondrial complex I. All the simulation and analysis codes and data are openly available and maintained in an online repository (Zenodo). Therefore, this paper has good data availablility and accessibility.

### Quality of experimental design
- The study design involves comparing a mutated protein structure with the original wildtype form. The molecular dynamics simulation generated enough data for statistical comparison.
- In terms of potential of research practice, it is unlikely that the authors performed the simulation and the analysis blinded. However, since the analysis codes are made publicaly available, questionable statistical manipulation is unlikely.

### Description of methods
In the paper itself, the simulation and analysis pipeline were only briefly described. It would be hard to reproduce the results based on the methods section; readers probably need to go into the available codes to pindown the exact steps.

### Description of sample population/data under study	
This study is examining the structural characteristics and chemical kinetics of mitochondrial complex I in wildtype form and a mutant form relevant to Leber's hereditary optic neuropathy. The mutant itself is relatively common in the disease population. The based structure used for simulation was obtained from cryo-EM data.

### Tool accessibility
Overall, this is an open access paper with all of its codes and data available for download online. The only practical barrier to reproduce the research would be limitations of computation resources.

## Paper 2 (RH): The morphology of an infarct in nonarteritic anterior ischemic optic neuropathy (2003)

### Data availability and accesibility
This paper presents a pathological examination of the optic nerve of an patient with nonarteritic anterior ischemic optic neuropathy. The raw processed pathological sample is probably kept at the institution, and the scanned pictures were included in the paper. However, the raw scanned pictures were not available online since it is a relatively old paper, from a time when online repository is not widely used.

### Quality of experimental design
There is no comparison with normal optic nerve sample in the paper. The pathologist probably knows the diagnosis of the patient, so analysis was not performed blinded.

### Description of methods
The pathological processing and image acquisition and processing were well-described in the paper. However, some details were omitted (such as the concentration of staining used), but this is typical practice in medical pathology papers.

### Description of sample population/data under study	
This paper is only based on one patient, since it is really hard to obtain patient samples with the rare disease.

### Tool accessibility
The pathological processing chemicals and microscopes are common in medical facilities and not expensive. However, patient sample would be really hard to obtain for such rare eye disease.

## Public Health

## Paper 1 (MS): Iron Replacement Therapy in the Routine Management of Blood Donors (2011)

### Data availability and accessibility
health data is very sensitive so reviewers would need permission from the ethics board of the hospital where the data was acquired from. The authors also do not mention the hospital where the data was collected; this information would have to be obtained by contacting the authors directly.

### Quality of experimental design
There was no mention of blinding or randomization in this study. Control donors were not matched for age, race, or gender

### Description of methods
 Laboratory testing protocol is sufficiently detailed.

### Description of sample population/data under study	
The exclusion criteria does not seem detailed enough. Depending on the location, blood donors can be given permanent deferrals based on their specific health history. In the paper, they do not mentions the local blood center donor eligibility criteria, and they also do not mention the location of the blood donation center. It would also be beneficial to specifically mention whether all blood donations in this study were allogenic or not.

### Tool accessibility
Neither the data collection software nor the data analysis software used in this study were mentioned, however this study did not employ computationally advanced analysis.

## Paper 2 (MS): Intravenous iron for the treatment of fatigue in nonanemic, premenopausal women with low serum ferritin concentration (2011)

### Data availability and accessibility
To access the data, reviewers would have to gain permissions from the local ethics committees of all participating hospital centers.

### Quality of experimental design
The research is double-blinded and the randomization method is described.

### Description of methods
The location of data collection was well described (and mentioned specific hospitals), however the time period that data was collected in was not described at all.
The laboratory method for measuring serum ferritin and hemoglobin concentration was not described.This study also included a "Short Performance Inventory" questionnaire, but there is not citation for where this questionnaire can be found, and neither is there detailed information on the content of the questionnaire.

### Description of sample population/data under study
There were also definitions in the inclusions and exclusion criteria that were not clearly described. There is ambiguity as to what the authors meant by "adequate contraception" in the inclusion criteria. Similarly, the exact "mental disorders" of the exclusion criteria were not mentioned, and neither was it described how they were assessed. The list of medications that would cause a participant to be unfit from participating in the study were also not thoroughly described.

### Tool accessibility
Neither the data collection software nor the data analysis software used in this study were mentioned. Otherwise, this study described the laboratory methods that they used.

## Paper 3 (MS): The effect of repeated blood donations on the iron status of male Saudi blood donors (2011)

### Data availability and accessibility
To access the data, reviewers would have likely have to gain permissions from the local ethics committees of all participating hospital centers.

### Quality of experimental design
There was no mention of blinding. Randomization didn't seem necessary due to study design.

### Description of methods
The lab methods are well described and both the location and time frame of data collection was described.

### Description of sample population/data under study
There is some ambiguity as to the replicability of this paper. It says "all donors were healthy", but it's unclear as to whether this was exclusion criteria for the study. If it is exclusion criteria, there needs to be a lot more detail on the diseases/conditions that would be reasons for exclusion.

### Tool accessibility
The data collection software and analysis software were described, however not in detail (the version of SPSS was not described, and the data collection software was described as "blood bank computer database", which provides little detail).




