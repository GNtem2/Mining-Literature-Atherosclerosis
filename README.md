# Mining-Literature-Atherosclerosis
Search PubMed for Gene associations with Atherosclerosis
packages lsa, pubmed.mineR, wordcloud
Atherosclerosis Biological Network. A Pubmed search was performed on 16/1/20 with term "atherosclerosis and inflammation". The file was downloaded as text file. 

R package: pubmed.mineR was used to search genes from HUGO Gene Nomenclature Committee. Latent semantic analysis was performed using a list of terms against the genes. The code is available in athero.Rmd. The data was saved as graphml file and exported to Gephi 0.9.2 for visualisation & community detection. 

Gephi: The node names need to be copy from Name column to Label column in Gephi data laboratory. The graph display is set to Fruchterman Reingold layout and run until the layout is stable. Next, the graph statistics are calculated using the tab 'statistics'. The 'modularity class' output is imported into 'Filter' under 'Attributes: Partition'. Following this, the node size is set according to degree centrality and the node color is set according to modularity class. The interactive graph was generated using  Sigma Exporter plugins in Gephi. Before visualisation, a manual editing step for the config.json file is required. 

Edit config.json: sigma: drawingProperties: labelThreshold change from 10 to 5; sigma:drawingProperties: defaultLabelSize change from 14 to 7. Click on the picture below to go to the interactive display; sigma: graphProperties: maxEdgeSize change from 0.5 to 4;  sigma: graphProperties: minEdgeSize change from 0.2 to 0.5; sigma: graphProperties: maxNodeSize change from 7 to 14.

[![here](./athero_community.png)](https://gntem2.github.io/Mining-Literature-Atherosclerosis/)


