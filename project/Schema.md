```mermaid
classDiagram

    class ChemicalGene{
    +PK id 
    chemicalname 
    chemicalid 
    casrn 
    genesymbol 
    geneid 
    organism 
    organismid 
    interaction 
    interactionactions}
    
    class ChemicalDisease{
    +PK id  
    chemicalid 
    diseasename 
    diseaseid 
    inferencescore}