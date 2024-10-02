# Genedex 
## Overview

Genedex is a Shiny application designed for genetic data exploration and visualization in the context of Alzheimer's Disease. It provides tools for managing gene lists, searching genes, calculating similarity matrices, analyzing facet interactions, performing pathway enrichment analysis, and conducting functional overlap analysis.

## Features

### Input Gene Lists:

- Add and visualize multiple gene lists for analysis.
  <img width="1470" alt="Screenshot 2024-08-29 at 9 53 27 PM" src="https://github.com/user-attachments/assets/78790a4c-111f-442f-90fe-541632097843">
 <img width="1470" alt="Screenshot 2024-08-30 at 1 39 47 PM" src="https://github.com/user-attachments/assets/41e6d2fd-ebf0-47e2-b1d9-08417bc2ca2a">


#### How to use Input Gene Lists
1) Navigate to the **"Input Gene Lists"** Tab:
    - Click on the **"Input Gene Lists"** option in the left sidebar menu.
2) Add a New Gene List:
    - Click the **"Add a Gene List"** button. This action will create a new entry form for a gene list.
    - In the **"Gene List Name"** field, enter a descriptive name for your gene list.
    - In the **"Gene List"** field, input the genes you wish to include, each on a new line.
3) Manage Gene Lists:
    - To remove a gene list, click the **"Remove Gene List"** button.
    - To add additional gene lists, click the **"+"** button to create more input fields.
4) Manage All Gene Lists:
    - Use the **"Clear All Gene Lists"** button to remove all gene lists you have added.
    - Click **"Save All Gene Lists"** to save the current gene lists for analysis.
    - Select **"Visualize Gene Lists"** to view a table containing the input gene list.

### Search:

- Gene search: Input a gene or a gene list to retrieve associated facets and related publications.
- Facet search: Select a facet from the drop-down menu to see the gene lists associated with that facet.

### How to use Search
<img width="1470" alt="Screenshot 2024-08-30 at 1 39 56 PM" src="https://github.com/user-attachments/assets/d674314c-f286-4e67-ba5e-606179e31f61">

 
#### How to use Gene Search

1) Enter Gene IDs:
   - In the **"Enter HUGO Gene IDs"** field, type one or more gene symbols separated by spaces. For example, you can enter ICAM1.
2) Upload a Gene List:
   - Alternatively, click the **"Browse…"** button to upload a text file containing HUGO Gene IDs. Ensure the file format is correct, with one gene per line or separated by spaces.
3) Select Input List:
   - Click the **"Use Input Gene List"** button to select from gene lists you have previously inputted or uploaded.
4) Search Genes:
   - After entering the gene IDs or uploading a file, click the **"Search Genes"** button to retrieve information about the genes.
5) Download Results:
   - Once the search is complete, click the **"Download Results"** button to download the results as a file for further analysis.
     
#### How to use Facet Search
1) Select a Facet:
   - Choose the facet of interest from the dropdown menu.
2) Search Facet:
   - After selecting a facet, click the **"Search Facet"** button to retrieve information about the selected facet.
  
### Similarity Matrix:

- Calculate and visualize a similarity matrix using the Jaccard index for selected facets or gene lists
- Display the similarity matrix as a heatmap.

### How to Use Similarity Matrix for Gene Lists:
  <img width="1470" alt="Screenshot 2024-08-29 at 9 54 07 PM" src="https://github.com/user-attachments/assets/9dd5d55c-30f0-4c94-9172-c4e5c78a9314">
  
1) Select Gene List:
   - **"Select Tags"** : Choose tags to filter gene lists containing the selected term.
   - **"Select Gene Lists"** : Choose a specific gene list by name from the dropdown menu.
   - **"Select Input Gene Lists"** : To add a gene list that you have previously inputted to the plot, select it from the dropdown menu.
2)  Generate plot:
    - Click **"Calculate"** to generate the similarity matrix.
    - Click **"Reset Plot"** to clear the current plot and start over.

 ### How to Use Similarity Matrix for Facets:
<img width="1470" alt="Screenshot 2024-08-29 at 9 54 17 PM" src="https://github.com/user-attachments/assets/db0e1ad7-3ccd-4f00-a22c-64b4c7f299c5">

1) **"Select Facets"**:
    - Use the dropdown menu to select the facets of interest or type them in manually.
    - Click **"Select All Facets"** to include all facets in the analysis.
    - Click **"Deselect All Facets"** to remove all selected facets from the analysis.
2) Generate plot:
    - Click **"Calculate"** to generate the similarity matrix.
    - Click **"Reset Plot"** to clear the current plot and start over.
    
### Facet Interactions:

- Visualize interactions between selected facets using a force-directed graph and an UpSet plot.
- Display overlapping genes between selected facets.

### How to Use Facet Interactions

#### Choose Analysis Type:
Select whether you want to perform the interaction analysis on Gene Lists or Facets.
1) Gene Lists: Analyze interactions based on the gene lists.
2) Facets: Analyze interactions based on the facets.

#### How to Use Facet Interaction for Gene Lists

<img width="1470" alt="Screenshot 2024-08-29 at 9 54 33 PM" src="https://github.com/user-attachments/assets/54ba05dc-7f92-445b-bc2c-8ec39fc89091">

1) Select Gene List:
   - **"Select Tags"** : Choose tags to filter gene lists containing the selected term.
   - **"Select Gene Lists"** : Choose a specific gene list by name from the dropdown menu.
   - **"Select Input Gene Lists"** : To add a gene list that you have previously inputted to the plot, select it from the dropdown menu.
2) Select your preferred visualization type:
  - Graph: Displays a network visualization of interactions.
  - Upset plot: Visualizes the intersections and overlaps between gene lists or facets. It allows you to visualize the genes in the overlapping sections by clicking on the bars and downloading the table.
3) Generate plot:
  - Click **"Calculate"** to generate the chosen visualization.
  - Click **"Reset Plot"** to remove the current visualization and start over.
  
  
#### How to Use Facet Interaction for Facets
 
<img width="1470" alt="Screenshot 2024-08-29 at 9 54 33 PM" src="https://github.com/user-attachments/assets/333e6c72-f3eb-4d32-a253-5cd5751ce38c">

1) **"Select Facets"**:
    - Use the dropdown menu to select the facets of interest or type them in manually.
    - Click **"Select All Facets"** to include all facets in the analysis.
    - Click **"Deselect All Facets"** to remove all selected facets from the analysis.
    - Click **"Select Input Gene Lists"** to add a gene list that you have previously inputted to the plot, select it from the dropdown menu.
2) Select your preferred visualization type:
  - Graph: Displays a network visualization of interactions.
  - Upset plot: Visualizes the intersections and overlaps between gene lists or facets. It allows you to visualize the genes in the overlapping sections by clicking on the bars and downloading the table.
3) Generate plot:
  - Click **"Calculate"** to generate the chosen visualization.
  - Click **"Reset Plot"** to remove the current visualization and start over.
  
