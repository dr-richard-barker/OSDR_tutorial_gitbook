---
description: >-
  Multi-study analysis is an advanced tool designed for analyzing and
  visualizing multiple RNA sequencing studies concurrently.
---

# Multi-study Page Overview

‌Selecting studies for Multi-study analysis:

* The multi-study page is used to initialize the parameters for data visualization of the multiple studies. Researchers can uncover intricate patterns of gene expression associated with specific conditions or treatments across a variety of experiments. Below are detailed instructions on how to effectively navigate and utilize the Multi-Study Page.
  * For your initial test, let's use rodent studies as an example.
  * Start by selecting "rodent" as the organism of interest. Since combining DNA microarray assays is not supported, ensure to filter by both "rodent" and "RNA sequencing" in the assay technology type.
  * Choose two different rodent studies that encompass various tissue types. For instance, select "OSD-49" and "OSD-100."
  * Mark the checkboxes beside the selected studies in the studies table.
  * Click the "Visualize Study" button to proceed.
  * In this example OSD-49 & OSD100 have been selected, normlized with DESeq2 and their first 2 principle components plotted in a 2D scatter plot. To the right the is a factor slectino tab where you can add new factors that will appear as columns beside the OSD-###. Clicking on the “Expand table” button reveals table showing all the replicates and the metadata the user loads.

<figure><img src=".gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

**Alt text:** Screenshot showing the graphical user interface of the Multi-study visualization application showing data for OSD-49 & OSD-100.



**‌Multi-study Data Normalization:**



A dialog box will appear to prompt you for data normalization options. The default selection is often "DESeq2" for normalization, but you can also choose "No Normalization."

* E-mail notification: If desired, you can enter your email address to receive a notification when the studies have been combined and normalized. Alternatively, proceed without entering an email address.
* Normalization and PCA Insights: Understand normalization details by clicking the Information button next to the normalization method. View the PCA chart, which provides insights into data distribution after normalization.
* Factor Selection and Differential Gene Analysis: Under "Factor Selection," choose variables to generate a factors table for differential gene analysis. Select parameters, characteristics, or factors from the dropdown list to add to the table.
* Exploring the Multi-Study Page: A PCA chart for data visualization will be included on the multi-study page. Utilize the PCA chart options to tailor your visualization based on specific criteria.
* Modifying Normalization Method: If you wish to change the normalization method (e.g., from "DESeq2" to "No Normalization"), click "Change Normalization Method."
* Sample Selection for Gene Expression Analysis: Select specific samples by clicking the "Select labeled, expand table" button. Choose samples based on factors added during factor selection.
* Visualizing and Downloading Results: Click "Visualize Studies" to proceed to visualization plots or download the accounts table. Depending on your selection, enter your email address for a notification upon completion.
*   Exploring Visualization Plots: Upon completion, the page will direct you to a range of visualization plots and graphs for your data analysis.

    \


    With these summarizes more comprehensive instructions, you are well-equipped to navigate the Multi-Study Page efficiently. This tool empowers you to analyze multiple RNA sequencing studies simultaneously, uncovering complex gene expression patterns and gaining valuable insights into your experimental data.

\
