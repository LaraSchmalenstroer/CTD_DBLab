# Biological Databases Lab 2022

## Group Project

## Proposal

ParkinsonDrugPredictor (PDP)

## Team members


1. Shubhi
2. Kriti
3. Zexin
4. Dmitry
5. Rohitha
6. Lara
7. Dhwani
8. Sanjana
9. Ana


## Context

## Introduction

### 1. State of the art


### 2. Background information
#### General information

Parkinson's disease is a neurodegenerative disorder that affects approximately 10 million people worldwide. Most patients that are diagnosed with Parkinson's disease are older than 50 years (~96 %). The likelihood of developing PD can be influenced by having certain genetic mutations in at least one of the parents. Depending on the particularly affected gene (see more in section Disease mechanisms), the inheritance patterns differ. 

The three main symptoms of Parkinson's disease, also referred to as parkinsonism, are
- tremor - shaking 
- bradykinesia - slowness of movement
- rigidity - muscle stiffness which can lead to cramps
Next to the above-mentioned main symptoms of PD, there are other physical and cognitive and psychiatric symptoms that might occur, such as: 
- physical symptoms:
  - balance problems
  - dizziness
  - sweating
- cognitive and psychiatric symptoms:
  - depression
  - anxiety
  - dementia

Source:
https://www.hopkinsmedicine.org/health/conditions-and-diseases/parkinsons-disease/the-genetic-link-to-parkinsons-disease
https://www.nhs.uk/conditions/parkinsons-disease/symptoms/ 


#### Disease mechanisms


In Parkinson's disease, there are many genes and pathways that are affected. Parkinson's Disease is a multifactorial disease, where both genetic and non-genetic, such as environmental factors, are involved. The most salient mechanisms involved in the development of Parkinson's Disease include:
+ Accumulation of misfolded proteins aggregates
  + Aggregation of alpha-synuclein (SNCA)
  + Hyper-phosphorylation of Tau
+ Genetic mutations
  + Parking, DJ-1 (PARK7)
  + PINK1 (PARK6)
  + LRRK2/PARK8
  + PARK3, PARK9, PARK10, and PARK11
  + Glucocerebrosidase (GBA) gene mutation 
+ Failure of protein clearance pathways
  + Ubiquitin-Proteasome System (UPS)
  + Molecular chaperones
  + Autophagy lysosomal pathway (ALP)
+ Mitochondrial damage
  + Mutation of mitochondrial DNA (mtDNA)
+ Oxidative stress
+ Excitotoxicity
+ Neuroinflammation

Source: https://translationalneurodegeneration.biomedcentral.com/articles/10.1186/s40035-017-0099-z#:~:text=The%20most%20salient%20mechanisms%20involved,6%2C%2013%2C%2070%5D.

#### Available drugs 

Until now, there is no cure for Parkinson's disease. 
But there are several drugs used to treat the symptoms of Parkinson's disease that can be ordered in six categories, all of which treat the symptoms targeting different proteins:
1. Levodopa

Levodopa is prescribed to PD patients because it is a precursor molecule of dopamine. While dopamine itself cannot cross the blood brain barrier, Levodopa can cross it and is then metabolized to dopamine by the DOPA decarboxylase. 
        
*Levodopa*, DrugBank Accession: _DB01235_. By synthesizing dopamine, the information flow in the brain is maintained so that movement can be executed in a control manner. Levodopa works as an agonist to the dopamine receptors D1 - D5. 
    
2. Dopamine agonists

Dopamine agonists stimulate the activity of the dopamine system by binding to the dopaminergic receptors. They do not have to be metabolized into dopamine. 

*Pramipexole*, DrugBank Accession: _DB00413_, is a non-ergot dopamine agonist drug, is used to treat tremor, rigidity, and bradykinesia (slow movement). It belongs to the class of small molecules and was first approved by the FDA in 1997. Although the mechanism is not fully understood yet it is thought that it stimulates dopamine receptors in the striatum of the brain. It is an agonist for the human D2, D3 and D4 dopamine receptor. 

3. Monoamine Oxidase B (MAO-B) inhibitors

MAO-B inhibitors work by inhibiting the enzymes involved in dopamine metabolism, here MAO-B.

*Safinamide*, DrugBank Accession: _DB06654_,is a small molecule that is used to treat Parkinson's disease since 2015 (Europe)/2017  (USA) as an add-on treatment to levodopa/carbidopa. It combines potent, selective, and reversible inhibition of MAO-B with blockade of voltage-dependent Na+ and Ca2+ channels and inhibition of glutamate release. It works as an antagonist to the human Amine oxidase (flavin-containing) B.

4. Catechol-O-methyl transferase inhibitors

*Tolcapone*, DrugBank Accession: _DB00323_, is a small molecule that is used in PD treatment in addition to the drug Levadopa. It inhibits the enzyme catechol-O-methyl transferase (COMT). The mechanism of action is still unknown but it is thought that its ability to inhibit COMT changes the plasma pharmacokinetics of levadopa and thus increases the concentration of levadopa in the plasma. 

5. Anticholinergics

Anticholinergics reduce the activity of the neurotransmitter acetylcholine, by acting as antagonists at cholinergic receptors. The loss of dopaminergic neurons results in a disturbed balance between dopamine and acetylcholine in the brain, and anticholinergic drugs may lead to restoration and maintenance of the normal balance between these two neurotransmitters. 

*Benzatropine*, DrugBank Accession: _DB00245_, belongs to the class of small molecules. It has anti-muscarinic and antihistaminic effects. Its main mechanism of action is the selective inhibition of dopamine transporters. 

6. Amantadine

Amantadine was first developed as an antiviral drug for treating flu and it is not known yet how it may have an effect on Parkinson's disease. 


Information in this section were taken from [DrugBank](https://go.drugbank.com/drugs/)
https://www.ncbi.nlm.nih.gov/books/NBK536726/ 


### Other software tools for drug prediction based on gene expression.
+ [MIT Clinical ML] (http://www.clinicalml.org/):  
    + [project](https://github.com/clinicalml/dgc_predict)
#### Description
'Predicting cell-specific drug perturbation profiles using available expression data from related conditions--i.e. from other drugs and cell types. We developed a computational framework that first arranges existing profiles into a three-dimensional array (or tensor) indexed by drugs, genes, and cell types, and then uses either local (nearest-neighbors) or global (tensor completion) information to predict unmeasured profiles.'     

+ DeSigN :  
    + [web tool](https://design-v2.cancerresearch.my/query)
#### Description
'Connecting gene expression with therapeutics for drug repurposing and development This web-based tool aims to predict drug efficacy against cancer cell lines using gene expression patterns. The algorithm correlates phenotype-specific gene signatures derived from differentially expressed genes with pre-defined gene expression profiles associated with drug response data (IC50) from 140 drugs' 




### 1. Problem or need


## Hypothesis

Tool to predict potential drugs for Parkinson's disease from Gene expression experiment data.


## Algorithm

1. Extract up and down regulated genes from the gene expression data. (Expression Atlas/ Microarray)
2. Get chemical data associated with the genes involved in the expression studies. (CTD)
3. Identify potential drugs based on the chemical data. (DrugBank/ChEMBL)

## Risks of implementation

1. Amount of data
2. Selection of gene expression experiments
3. Extracting correct Gene ID(s)
4. Missing information
5. Compounds vs Drugs


## Material and Methods 

### Software libraries

+ Pandas
+ Numpy
+ SQLAlchemy
+ pymysql
+ File parsers
+ Modules for APIs
+ MySQLWorkbench

### RDBMS
MySQL

### Programming language
Python 3.9


### Databases
+ Expression Atlas
+ some useful links:
    + [Expression Atlas ftp](http://ftp.ebi.ac.uk/pub/databases/microarray/data/atlas/experiments/)
+ Microarray
+ [CTD](http://ctdbase.org/)
  + CTD is a database that combines data about genes, pathways, chemicals, drugs and diseases
  + includes several tables regarding terminology
  + organized in 18 tables
  + current release: March 2022
  + some useful links:
    + [ctd schema](https://pyctd.readthedocs.io/en/latest/_images/all.png)
    + [downloads](http://ctdbase.org/downloads/)
    + [help](http://ctdbase.org/help/)
+ DrugBank
+ ChEMBL





