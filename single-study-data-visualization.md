---
description: Launching the single-study data visualization
---

# Single Study Data Visualization

Alternatively, if you’ve identified a study of interest in the OSDA and it has processed data available then you can view it with the OSDR single study data Visualization either by launching it from the OSDR accession’s ”Visualization” button or by replacing the \* wildcards in this website URL ([https://visualization.genelab.nasa.gov/data/OSD-\*\*\*](https://visualization.genelab.nasa.gov/data/OSD-\*\*\*)) with the accession number of interest.

*   After assessing the title, study descriptions and any related research paper you can use the data visualization application to learn more about some of the quantitative patterns within the data.

    * **Single study** [**example OSD-37:**](https://visualization.genelab.nasa.gov/data/OSD-37) If you’ve already navigated to a study of interest by searching through the study metadata you can launch the visualization menu using the visualization tab on the left menu.&#x20;



<figure><img src=".gitbook/assets/Slide21.png" alt="Example showing the OSD page for accession # 37. The page presents a description of the experiment and related metadata. https://osdr.nasa.gov/bio/repo/data/studies/OSD-37."><figcaption><p><em>Example showing the OSD page for accession # 37. The page presents a description of the experiment and related metadata.</em> <a href="https://osdr.nasa.gov/bio/repo/data/studies/OSD-37">https://osdr.nasa.gov/bio/repo/data/studies/OSD-37</a>.</p></figcaption></figure>

### &#x20;<a href="#bltxtycjg7o9" id="bltxtycjg7o9"></a>

### Single Study Visualization Navigation bar <a href="#bltxtycjg7o9" id="bltxtycjg7o9"></a>

**The OSDR Visualization Navigation bar can allow you to navigate to a graph of interest.**

* After launching the OSDR visualization application on the lefthand side of the screen you’ll see a navigation window that will allow you to select to go to the "Home," "PCA," "Volcano,", “Pair plots”, “Heat maps”, “DGE”, “GSEA”, and Group Selection.
  * [**Single study navigation example**](https://visualization.genelab.nasa.gov/data/OSD-37)**:** In this example, we see Group 1 of Col-0\&FLT ( FLT is the flight group) and Group 2 is Col-0\&GC (GC is the ground control group). [https://visualization.genelab.nasa.gov/data/OSD-37](https://visualization.genelab.nasa.gov/data/OSD-37)
  * Clicking on these visualisation names allows the user to jump straight to the visualization of most interest.

<figure><img src=".gitbook/assets/Slide33.png" alt="The OSDR Visualization interface includes the text &#x22;OSDR Visualization&#x22; and &#x22;OSD-37,&#x22; and a “Study details” search bar. Below is a horizontal navigation menu with various options like &#x22;Home,&#x22; &#x22;PCA,&#x22; &#x22;Volcano,&#x22;, “Pair plots”, “Heat maps”, “DGE”, “GSEA”, and “Group Selection”. In this example, it shows that Group 1 of Col-0&#x26;FLT (which is the flight group) and Group 2 is Col-0&#x26;GC (which is the ground control group). There is a “Modify groups” button in the bottom left corner that can be used to change the groups of samples used to generate the data in the plots" width="140"><figcaption><p><em>The OSDR Visualization interface includes the text "GeneLab Visualization" and "OSD-37," and a “Study details” search bar. Below is a horizontal navigation menu with various options like "Home," "PCA," "Volcano,", “Pair plots”, “Heat maps”, “DGE”, “GSEA”, and “Group Selection”. In this example, it shows that Group 1 of Col-0&#x26;FLT (which is the flight group) and Group 2 is Col-0&#x26;GC (which is the ground control group). There is a “Modify groups” button in the bottom left corner that can be used to change the groups of samples used to generate the data in the plots</em></p></figcaption></figure>

### &#x20;<a href="#hmtojdhstykw" id="hmtojdhstykw"></a>

### Select Group(s) <a href="#hmtojdhstykw" id="hmtojdhstykw"></a>

**Select Groups can be compared statically using the GeneLab data visualisation application.**

* Space Flight (FLT) vs Ground control (GC) is a linear model often used to understand and identify genes, proteins and other omics data types that change in response to spaceflight (or related stimuli)
  * **Single study grouping example:** Select the sample group 1 and group 2 for differential comparison. You can deselect these groups by clicking on the blue check box or select them by clicking on the empty boxes. In this example, the user can compare the ecotype and treatment groups.

<figure><img src=".gitbook/assets/Slide49.png" alt="The images show the Group Selection screen. The screen is divided into two sections, each labelled with a group name and containing descriptions of the selected factors. In this example, it shows the &#x22;Ecotypes” and &#x22;treatments&#x22;. A red dashed line highlights that when 2 groups are assigned a pop-up window shows the groups that are being compared."><figcaption><p><em>The images show the Group Selection screen. The screen is divided into two sections, each labelled with a group name and containing descriptions of the selected factors. In this example, it shows the "Ecotypes” and "treatments". A red dashed line highlights that when 2 groups are assigned a pop-up window shows the groups that are being compared.</em></p></figcaption></figure>

### &#x20;<a href="#we9brgzii034" id="we9brgzii034"></a>

### Principal component analysis <a href="#we9brgzii034" id="we9brgzii034"></a>

**Principal component analysis (PCA) shows clusters of samples based on their similarity.**

* **PCA:** Click on samples to the right to select the desired samples to be viewed on the PCA plot. Icons on the upper right region of the plot allow for downloading, navigating and saving the plot. You can choose either 2D or 3D plots. If you click on the 3D graph and hold the left mouse button you can rotate the graph in 3D to optimise the angle and potentially highlight specific clustering patterns.
  * **Single study PCA example:** 3D plot has been selected and PC1, PC2, and PC3 are presented on the graph. Drop-down options allow users to replace these PC’s by selecting an alternative from the menu.
  * We can also see next to the “Color by factor” label that the current “all” is selected and the yellow arrow shows how the names of the factors have been combined in the figure legend.
  * It can be important to explore the PC's that separate the data based on different factors as the main factor such as spaceflight might not always be captured by the first or second PC's values. Sometimes results presented as a series of 2D PCA plots can be clearer than a 3D plot present 3 PC values.&#x20;

<figure><img src=".gitbook/assets/Slide34.png" alt="The scatter plot exemplifies the clustering of samples via Principal Component Analysis (PCA), a method that transforms correlated variables into uncorrelated ones called principal components. The plot presents the projection of samples onto the first two or 3 principal components, showcasing the majority of the variance in the original data. The clustering suggests the presence of distinct groups, indicating different characteristics captured by the principal components."><figcaption><p><em>The scatter plot exemplifies the clustering of samples via Principal Component Analysis (PCA), a method that transforms correlated variables into uncorrelated ones called principal components. The plot presents the projection of samples onto the first two or 3 principal components, showcasing the majority of the variance in the original data. The clustering suggests the presence of distinct groups, indicating different characteristics captured by the principal components.</em></p></figcaption></figure>

#### &#x20;<a href="#eewgwyi97mqc" id="eewgwyi97mqc"></a>

### Pair plots  <a href="#eewgwyi97mqc" id="eewgwyi97mqc"></a>

**The “Pair plots” can be used to compare 2 samples from group 1 or group 2 respectively.**

* Drop-down menus allow the researcher to select different replicates and view the comparative gene expression dispersion plots. This is useful for finding outlining samples or loci and the difference between each sample can be refined by adjusting the color threshold (default 20). In the top right-hand corner, there is a menu of graph-specific options, including snapshot, zoom, lasso, and full screen. The “update” button is highlighted in blue and needs to be pressed if you change any of the factors.
  * **Pair plot replicate comparison example:** We can see the % difference threshold is set to 20, we can also see the names of the samples being paired against one another and they are replicated of the same treatment.

<figure><img src=".gitbook/assets/Slide35 (1).png" alt="Pair plots comparing 2 samples from Atha_Col-0_s1-pool_FLT_Rep4_R1-FL-B4 on the X axis and with Atha_Col-0_s1-pool_FLT_Rep4_R1-FL-B4 on the Y-axis. Loci are represented by red and blue dots. In the top right-hand corner, there is a menu of options, including snapshot, zoom, lasso, full screen, and the “update” button is highlighted in blue."><figcaption><p><em>Pair plots comparing 2 samples from Atha_Col-0_s1-pool_FLT_Rep4_R1-FL-B4 on the X axis and with Atha_Col-0_s1-pool_FLT_Rep4_R1-FL-B4 on the Y-axis. Loci are represented by red and blue dots. In the top right-hand corner, there is a menu of options, including snapshot, zoom, lasso, full screen, and the “update” button is highlighted in blue.</em></p></figcaption></figure>

### &#x20;<a href="#id-3cb9r7if7di1" id="id-3cb9r7if7di1"></a>

### Volcano Plots <a href="#id-3cb9r7if7di1" id="id-3cb9r7if7di1"></a>

**Volcano plots show statistical significance vs magnitude of change.**

* To present the Volcano plot, the p-value is converted using a -log10 transformation to enhance the visibility of significant loci. The Fold Change (FC) is transformed using a Log2 transformation to balance the representation of upregulated and downregulated genes. This facilitates the identification of genes with significant statistical differences and substantial expression changes. Users can select parameters, samples for comparison, and the maximum adjusted p-value using the drop-down menu. The Log2 FC threshold can be adjusted using the menu bar at the top. The image can be exported or explored using the Zoom or Lasso tool to investigate specific clusters or outliers.
  * **Volcano plot example:** This graph generated by OSD-37 shows the adjusted P-value on the y-axis after it has experienced a -log10 transformation compared to the Log10 fold change (FC). In this example, _SCPL50_ appears to have a dramatic suppression during flight.

<figure><img src=".gitbook/assets/Slide36.png" alt="Image showing a volcano plot, with red dots representing genes with a significant increase in expression in orbit and blue dots representing genes that expression that was potentially suppressed by spaceflight-related factors. Drop-down menu allows for the selection of parameters, samples for comparison and maximum adjusted p-value. Some tabs also enable the transformation of the Y axis, the threshold of the adjusted P-value and the threshold of the Log2 FC can be adjusted using the menu bar at the top."><figcaption><p><em>Image showing a volcano plot, with red dots representing genes with a significant increase in expression in orbit and blue dots representing genes that expression that was potentially suppressed by spaceflight-related factors. Drop-down menu allows for the selection of parameters, samples for comparison and maximum adjusted p-value. Some tabs also enable the transformation of the Y axis, the threshold of the adjusted P-value and the threshold of the Log2 FC can be adjusted using the menu bar at the top.</em></p></figcaption></figure>

#### &#x20;<a href="#t7933tpb5wrd" id="t7933tpb5wrd"></a>

### Table of gene expression data <a href="#t7933tpb5wrd" id="t7933tpb5wrd"></a>

**A summary table of data compiling gene RefSeq IDs, Symbols, Log2Fc, P values, and Adjusted-P-values is often the most concise way to view data.**

* In the top right-hand corner, boxes allow the user to filter the table based on the maximum P-VAL (P-value), maximum ADJP (adjusted P-value), LOG2FC (Log2 transformed fold change) or to just search for gene REFSEQ ID or gene Symbol (Name). In the top left of the table, the buttons allow the user to copy, export to CVS, Excel, PDF or even directly Print.
  * **Summary of results example:** This table shows the top 10 most significantly differentially expressed loci from OSD-37. The maxim adjusted p-value is set to 0.05, in the bottom left it shows 2445 entries selected by this threshold, in the bottom right it shows that there are 245 pages of data (as the screen had been adjusted to show 10 loci per page). These can be downloaded for further analysis.

<figure><img src=".gitbook/assets/Slide38.png" alt="A screenshot from OSDR data visualization titled &#x22;OSD-37 DGE&#x22; showing a list of Gene REFSEQ IDs and Gene Symbols, along with their LOG2FC, PVAL and ADJP values. In the top right corner, there are boxes where users can enter values for P-VAL (P-value), maximum ADJP (adjusted P-value), LOG2FC (Log2 transformed fold change) or just search for particular gene REFSEQ ID or gene Symbol (Name). In the top left, there are a series of buttons to help export to CVS, Excel, PDF or Print. In the bottom left corner, it shows the number of entries on the page the total number selected by the filtering options and the total number of entries. In the bottom right corner, some buttons allow the user to navigate through the results on the screen."><figcaption><p><em>A screenshot from OSDR data visualization titled "OSD-37 DGE" showing a list of Gene REFSEQ IDs and Gene Symbols, along with their LOG2FC, PVAL and ADJP values. In the top right corner, there are boxes where users can enter values for P-VAL (P-value), maximum ADJP (adjusted P-value), LOG2FC (Log2 transformed fold change) or just search for particular gene REFSEQ ID or gene Symbol (Name).</em> <em>In the top left, there are a series of buttons to help export to CVS, Excel, PDF or Print. In the bottom left corner, it shows the number of entries on the page the total number selected by the filtering options and the total number of entries. In the bottom right corner, some buttons allow the user to navigate through the results on the screen.</em></p></figcaption></figure>

### Gene Set Enrichment Analysis (GSEA) <a href="#l6v0c891a6ps" id="l6v0c891a6ps"></a>

**GSEA is a tool that enables statistical comparisons of genetic and molecular databases.**

[“Geneset Enrichment Analysis](https://www.gsea-msigdb.org/gsea/index.jsp) (GSEA) - For a detailed explanation of GSEA statistics (ES, NES, FDR, P-value) see the [\*GSEA Statistics](https://www.gsea-msigdb.org/gsea/doc/GSEAUserGuideTEXT.htm#\_Enrichment\_Score\_\(ES\)) website. GSEA is performed using GSEApy 0.10.3, for more information about the parameters used and how to run GSEApy GSEA function: [GSEA](https://gseapy.readthedocs.io/en/latest/run.html) or [GSEApy documentation](https://gseapy.readthedocs.io/en/latest/introduction.html). All gmt files were downloaded from Enrichr: [Enrichr libraries](https://maayanlab.cloud/Enrichr/#libraries). The number of “genesets” and maximum false discovery rate (FDR) are set to their default values 6 and 0.25 respectively. The Permutations, type, min size and max size are all left as default.

* The are many plot types that be used to view these results including, Enrichment Score Plot, NES Plot, Dot Plot, Ridge Ploy and Network Plot.
  * **Example GSEA:** Before starting the analysis select the plot type you wish to use. This example uses a NES Plot (bar plot) but there are often logical reasons to present different types of data in different types of plot(s) to help disguise between results.

<figure><img src=".gitbook/assets/Slide39.png" alt="Image displaying a table of graphing options. The selection of options has created a red NES plot showing 4 terms (Ribosome, Endocytosis, RNA degradation and cell cycle) identified by GSEA analysis of the KEGG_2019 database. The permutation and gene list min and maximum parameters are highlighted with an orange dashed box. The plot-type menu has been highlighted with an orange dotted box."><figcaption><p><em>Image displaying a table of graphing options. The selection of options has created a red NES plot showing 4 terms (Ribosome, Endocytosis, RNA degradation and cell cycle) identified by GSEA analysis of the KEGG_2019 database. The permutation and gene list min and maximum parameters are highlighted with an orange dashed box. The plot-type menu has been highlighted with an orange dotted box.</em></p></figcaption></figure>

#### &#x20;<a href="#o9we3slvz8rf" id="o9we3slvz8rf"></a>

### Ontology databases and statistical methods used for analysis. <a href="#o9we3slvz8rf" id="o9we3slvz8rf"></a>

**Selecting different databases for statistical analysis can identify different responses and provide alternative perspectives and insights from the results.**

* Numerous ontology databases and statistical methodologies are available for application to the processed DESeq2 results.
  * **Ontology database example description:** A menu of pop-up menu databases can be opened and one selected based on your model organism and question of choice. 5 different statical methods can be used by GSEA, signal to noise, T test, Fold change, Difference of class and Log2 Fold change.

<figure><img src=".gitbook/assets/Slide40.png" alt="Image of half of the OSDR visualization page, the “Gene Set” menu has KEGG_2019 selected and a red dotted line links the list of accessible databases that can be selected from the connected drop-down menu that is highlighted by a yellow dotted line. The image also shows a red dashed line listing the different analysis “Methods” that can be used and the “Fold change” option is highlighted in blue to show it is selected." width="563"><figcaption><p><em>Image of half of the OSDR visualization page, the “Gene Set” menu has KEGG_2019 selected and a red dotted line links the list of accessible databases that can be selected from the connected drop-down menu that is highlighted by a yellow dotted line. The image also shows a red dashed line listing the different analysis “Methods” that can be used and the “Fold change” option is highlighted in blue to show it is selected.</em></p></figcaption></figure>

#### &#x20;<a href="#bj3385d7e61m" id="bj3385d7e61m"></a>

### Dot plots <a href="#bj3385d7e61m" id="bj3385d7e61m"></a>

**Dot plots can present 3 types of data on the same graph.**

The OSDR facilitates the visualization of the normalized enrichment score, false discovery rate, and Gene ratio values of all differentially expressed pathways on a single graph for user evaluation.

* **Phenotype Permutation vs. Gene Set Permutation:** Choosing the appropriate permutation method can influence your results. Phenotype permutation is generally preferred as it maintains the biological context of your experiment.
  * **Example dot plot:** demonstrating the analysis of the OSD-37 KEGG\_2019 pathway employing the Fold change method and “Phenotype” permutation type. The Minimum and maximum size parameters were retained at their default values of 15 and 500 loci, respectively, as per standard practice. The quantities of “geneset”s” and the maximum false discovery rate (FDR) are set to their default values of 6 and 0.25, respectively.

<figure><img src=".gitbook/assets/Slide41.png" alt="A screenshot of an Open Science Data Repository (OSDR) webpage. The page displays a Dotplot graph titled &#x22;OSD-37 GSEA.&#x22; The x-axis label is &#x22;Normalized /enrichment Score&#x22; and the y-axis shows the name of the enriched KEGG pathway. The graph used two colors, red and blue to emphasize the variation in the FDR values for this data series. Data points size displays the Gene ratio value which is connected by lines to the pathway name on the Y-axis. Red dotted lines highlight where the Dot ploy options can be found and that in this example the “Phenotype” permutation has been selected."><figcaption><p><em>A screenshot of  a Dotplot graph titled "OSD-37 GSEA." The x-axis label is "Normalized /enrichment Score" and the y-axis shows the name of the enriched KEGG pathway. The graph used two colors, red and blue to emphasize the variation in the FDR values for this data series. Data points size displays the Gene ratio value which is connected by lines to the pathway name on the Y-axis. Red dotted lines highlight where the Dot ploy options can be found and the “Phenotype” permutation has been selected.</em></p></figcaption></figure>





### Ridge plots <a href="#zc2ql3hfusf9" id="zc2ql3hfusf9"></a>

**A ridge plot combines a density plot and a histogram to show how data, like Fold Change (FC), is distributed.**

The OSDR facilitates the visualization of the false discovery rate (FDR), and Foldchange values of all differentially expressed pathways on a single graph for user evaluation. This visualization aids in determining whether genes are predominantly upregulated, downregulated, or exhibit minimal change. The smooth, ridge-like form reveals trends, and the plot is compatible with log-transformed data, a common feature in fold-change analysis. Overlaying plots for various groups allows researchers to compare fold-change distributions.

* Ridge plots are effective tools for present GSEA analysis.
  * **Example Ridge plot:** This example ridge-plot was made with a “Fold Change” of loci from the KEGG\_2019 GSEA analysis data from OSD-37. The Minimum size and maximum size values were left to the default 15 and 500 loci as standard. The number of ““geneset”s” and maximum false discovery rate (FDR) are set to their default values 6 and 0.25 respectively.

<figure><img src=".gitbook/assets/Slide42.png" alt="A screenshot of an Open Science Data Repository (OSDR) ridge plot page displays a ridge plot entitled &#x22;OSD-37 GSEA”. The Y-axis label shows the names of the terms detected by enrichment analysis of the selected gene sets eg Endocytosis and Cell cycle. The x-axis label is &#x22;Gene Fold Change”. Red dotted line highlights where the “Ridge Plot&#x22; option was engaged."><figcaption><p><em>A screenshot of an Open Science Data Repository (OSDR) ridge plot page displays a ridge plot entitled "OSD-37 GSEA”. The Y-axis label shows the names of the terms detected by enrichment analysis of the selected gene sets eg Endocytosis and Cell cycle. The x-axis label is "Gene Fold Change”. Red dotted line highlights where the “Ridge Plot" option was engaged.</em></p></figcaption></figure>

### &#x20;<a href="#v5vfnpxc0gtj" id="v5vfnpxc0gtj"></a>

### Network Plot <a href="#v5vfnpxc0gtj" id="v5vfnpxc0gtj"></a>

**A network plot uses dots that represent nodes of data points that describe the response detected in the analysis.**

* Network plots are effective tools for showing the variation in the number of genes involved in a detected response.
  * **Example network diagram:** it can be observed that the Ribosome possesses a greater number of loci that were implicated in that response ontology group. Even though "RNA degradation" and "Cell cycle" demonstrate a lesser quantity of associated genes, it is evident that they possess heightened significance due to their diminished adjusted P-value, as delineated by the gradient ranging from blue to red.

<figure><img src=".gitbook/assets/Slide43.png" alt="A screenshot of an Open Science Data Repository (OSDR) network plot page with the title OSD-37 GSEA. In the center a plot shows 4 circles, representing enriched terms from the KEGG_2019 database. The size of the dots indicates the number of genes detected in that GO group and the red-to-blue color gradient shows the significance of their enrichment. A red dotted line highlights where the network plot was selected"><figcaption><p><em>A screenshot of an Open Science Data Repository (OSDR) network plot page with the title OSD-37 GSEA. In the center a plot shows 4 circles, representing enriched terms from the KEGG_2019 database. The size of the dots indicates the number of genes detected in that GO group and the red-to-blue color gradient shows the significance of their enrichment. A red dotted line highlights where the network plot was selected</em></p></figcaption></figure>

####

### Network Plot used in conjunction with pathway illustration

**A network plot uses dots that represent nodes of data points that describe the response detected in the analysis.**

* Network plots can be merged with pathway diagrams to help illustrate connections between enriched terms and concepts like cellular function. Figures can then be shared with other OSDR AWG collaborators on platforms like GitHub as staging for eventual publication in Zenodo and peer-reviewed journals.

<figure><img src=".gitbook/assets/Slide44.png" alt="The previous network dots and plot information have been incorporated into the endocytosis diagram to illustrate how these KEGG pathway terms related to cellular biology. The use of pop-out boxes and dotted or dashed lines is used to show connections based on knowledge from the literature."><figcaption><p><em>The previous network dots and plot information have been incorporated into the endocytosis diagram to illustrate how these KEGG pathway terms related to cellular biology. The use of pop-out boxes and dotted or dashed lines is used to show connections based on knowledge from the literature.</em></p></figcaption></figure>

### &#x20;<a href="#j5wz6ra5953b" id="j5wz6ra5953b"></a>

### NES plots <a href="#j5wz6ra5953b" id="j5wz6ra5953b"></a>

**NES (Normalized Enrichment Score) plot offers a visual representation of the normalized enrichment score for gene sets identified by the user based on their parameters.**

* NES plots are an effect tool for viewing pathways that are identified by GSEA.
  * **Example NES plot:** The data from OSD-37 provides the normalized enrichment score adjacent to terms that possess enrichment in the selected database. KEGG\_2019 was used as the “geneset” for enrichment analysis. However, in this instance, we show it is possible to change the database analyzed. The bar plot then displays GO terms identified during the analysis when the GO\_cellular\_Componet\_AutoRIF gene set database was queried.

<figure><img src=".gitbook/assets/Slide45 (1).png" alt=""><figcaption><p><em>This image shows a NES plot and the options used to generate it. Situated at the top of the webpage is a search bar that facilitates the exploration of specific terms within the datasets and other “geneset" for analysis. Immediately beneath the search mechanism is a tabular structure providing alternative plot types and graph parameters. The bar plot structure summarizes distinct gene groups that are known to function in a similar location based on the GO-Cellular_Component_AutoRIF enrichment analysis. The Red dotted lines highlight the “number of “geneset”s” and the method values have been adjusted from their default values.</em></p></figcaption></figure>





### Enhancing NES plots

**Adjusting the parameters to influence the quantity and sequence of pathways detected.**

* NES plots have a numerical constant that can be adjusted to modify the appearance pathways that are identified by GSEA
  * **Numerical method example:** In this OSD-37 example we’ve changed the “Method” value to 0 (classic), which changes the normalized enrichment score and graph layout.

<figure><img src=".gitbook/assets/Slide46.png" alt="This image shows a screenshot from the OSDR Visualization software showing an NES plot graph and the options used to generate it. The bar plot structure summarizes distinct gene groups that are known to function in a similar location based on the GO-Cellular_Component_AutoRF enrichment analysis. The red dotted line highlights that the “Method” is currently set to 0 (classic mode) but was set to 1 in the previous figure."><figcaption><p><em>This image shows a NES plot and the options used to generate it. The bar plot structure summarizes distinct gene groups that are known to function in a similar location based on the GO-Cellular_Component_AutoRF enrichment analysis. The red dotted line highlights that the “Method” is currently set to 0 (classic mode) but was set to 1 in the previous figure.</em></p></figcaption></figure>



**Refining NES plots using the Method Value**

**Adjusting the “geneset” is highly recommended in the Method tab and can change the number and order of pathways identified.**

* When utilizing a normalized enrichment score plot (NES plot) to depict pathway enrichment via the fold change method, the graphical representation not only illustrates pathways with statistical significance but incorporates pathways that lack such significance.
  * **Number of “genesets” example:** In this example, the “Method” value is set to 1, and we’ve changed the “geneset” to Cellular\_Component\_AutoRIF\_Predicted\_zscore. Notice that the number of “genesets” is now set to 15 and that the color coding shows that only 4 of these are significant based on the current threshold of a maximum False Discovery Rate of 0.25.

<figure><img src=".gitbook/assets/Slide47.png" alt="This image displays a screenshot of the OSDR Visualization software, which includes an NES plot graph and the parameters used to create it. The NES bar plot structure summarizes distinct gene groups known to function in a similar cellular location based on GO-Cellular_Component_AutoRIF_zscore enrichment analysis. The method is currently set to 0 1, and the number of “geneset”s included was set to 15, with coloring determined by a 0.25 False Discovery Rate (FDR) cutoff threshold. Red arrows highlight the Gene sets and number of “geneset”s selected for this enrichment analysis."><figcaption><p><em>This image displays a screenshot of the OSDR Visualization software, which includes an NES plot graph and the parameters used to create it. The NES bar plot structure summarizes distinct gene groups known to function in a similar cellular location based on GO-Cellular_Component_AutoRIF_zscore enrichment analysis. The method is currently set to 0 1, and the number of “geneset”s included was set to 15, with coloring determined by a 0.25 False Discovery Rate (FDR) cutoff threshold. Red arrows highlight the Gene sets and number of “geneset”s selected for this enrichment analysis.</em></p></figcaption></figure>



### Fine-tuning permutations

**Adjusting the permutation value can be used to improve the GSEA statistical model.**

GSEA calculates enrichment scores by comparing the data to a random null distribution. This null distribution is generated by permuting the phenotype labels of your samples numerous times. A higher number of permutations leads to a more precise estimation of the p-value associated with your enrichment score.

* You can choose the number of permutations to run, with a higher number leading to potentially more accurate p-values.
  * **Example Finetuning Permutations:** Altering the default premonition from 300 to 500 in the example description resulted in a significant change in the FDR of the "cytoskeleton" Gene Ontology term.

<figure><img src=".gitbook/assets/Slide48.png" alt="This image displays a screenshot of the GeneLab Visualization software, which includes an NES plot graph and the parameters used to create it. The NES bar plot structure summarizes distinct gene groups known to function in a similar cellular location based on GO-Cellular_Component_AutoRIF_zscore enrichment analysis. The method is currently set to 1, and the number of “geneset”s included was set to 15, with coloring determined by a 0.25 False Discovery Rate (FDR) cutoff threshold. The permutations number has been increased to 500 and the cytoskeleton GO term has increased its NES score and changed from the Red FDR>0.25 to the Blue FDR<0.25 group. Red arrows highlight the Permutations value has been increased and that moving the mouse over a bar creates a popup that provides its name and value."><figcaption><p><em>This image displays NES plot graph and the parameters used to create it. The NES bar plot structure summarizes distinct gene groups known to function in a similar cellular location based on GO-Cellular_Component_AutoRIF_zscore enrichment analysis. The method is currently set to 1, and the number of “genesets” included was set to 15, with coloring determined by a 0.25 False Discovery Rate (FDR) cutoff threshold. The permutations number has been increased to 500 and the cytoskeleton GO term has increased its NES score and changed from the Red FDR>0.25 to the Blue FDR&#x3C;0.25 group. Red arrows highlight the permutation value has been increased and that moving the mouse over a bar creates a popup that provides its name and value.</em></p></figcaption></figure>

### &#x20;<a href="#xez5bpa6ns59" id="xez5bpa6ns59"></a>
