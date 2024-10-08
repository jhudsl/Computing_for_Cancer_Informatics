---
title: "Data Management Platforms and Systems"
output: html_document
---




# Data Management Platforms and Systems

In this chapter we will provide examples of data management systems that you might find useful for your research. Please note that we aim to provide a general overview of options and thus this is not a complete list. Let us know if there is a platform or system that you think we should include!

<img src="resources/images/05-Specific_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf5f8818810_1_171.png" title="Learning Objectives: 1.Recognize general informatics computing and data management platforms. 2.Be aware of specific genomics data management systems 3.Be aware of specific imaging data management systems  4.Be aware of specific clinical data management systems" alt="Learning Objectives: 1.Recognize general informatics computing and data management platforms. 2.Be aware of specific genomics data management systems 3.Be aware of specific imaging data management systems  4.Be aware of specific clinical data management systems" width="100%" style="display: block; margin: auto;" />

## General Platforms

We will start out with more general platforms, that allow you flexibility to perform analyses with a variety of types of data. 

## Galaxy

This section was written by [Jeremy Goecks](https://goeckslab.org/people/jeremy.html):

Galaxy is a web-based computational workbench that connects analysis tools, biomedical datasets, computing resources, a graphical user interface, and a programmatic API. Galaxy (https://galaxyproject.org/) enables accessible, reproducible, and collaborative biomedical data science by anyone regardless of their informatics expertise. There are more than 8,000 analysis tools and 200 visualizations integrated into Galaxy that can be used to process a wide variety of biomedical datasets. This includes tools for analyzing genomic, transcriptomic (RNA-seq), proteomic, metabolomic, microbiome, and imaging datasets, tool suites for single-cell omics and machine learning, and thousands of more tools. Galaxy’s graphical user interface can be used with only a web browser, and there is a programmatic API for performing scripted and automated analyses with Galaxy.

<img src="resources/images/05-Specific_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_131.png" title="Galaxy can be accessed through a web browser and provides users with access to tools, datasets, computing resources, a graphical user interface (GUI) for users who would like to interact with Galaxy by clicking buttons and using drop-down menus and a programmtic API for users that would like to write code to interact with Galaxy" alt="Galaxy can be accessed through a web browser and provides users with access to tools, datasets, computing resources, a graphical user interface (GUI) for users who would like to interact with Galaxy by clicking buttons and using drop-down menus and a programmtic API for users that would like to write code to interact with Galaxy" width="100%" style="display: block; margin: auto;" />

Galaxy is used daily by thousands of scientists across the world. A vibrant Galaxy community has deployed hundreds of Galaxy servers across the world, including more than 150 public and three large national/international servers in the United States, Europe, and Australia (https://usegalaxy.org, https://usegalaxy.eu, https://usegalaxy.org.au). The three national/international servers have more than 250,000 registered users who execute >500,000 analysis jobs each month. Galaxy has been cited more than 10,000 times with >20% from papers related to cancer. The Galaxy Tool Shed (https://usegalaxy.org/toolshed) provides a central location where developers can upload tools and visualizations and users can search and install tools and visualizations into any Galaxy server. Galaxy has a large presence in the cancer research community. Galaxy serves as an integration and/or analysis platform for 7 projects in the NCI ITCR program. There is also increasing use of Galaxy in key NIH initiatives such as the NCI Cancer Moonshot Human Tumor Atlas Network (HTAN) and the NHGRI Data Commons, called the AnVIL (https://anvilproject.org/).

<img src="resources/images/05-Specific_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_135.png" title="Map of the 3 Galaxy servers" alt="Map of the 3 Galaxy servers" width="100%" style="display: block; margin: auto;" />


Galaxy’s user interface, accessible via a web browser, provides access to all Galaxy functionality. The main Galaxy interface has three panels: available tools (left), running analyses and viewing data (middle), and a full history of tools run and datasets generated (right). 

<img src="resources/images/05-Specific_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_111.png" title="Galaxy user interface showing the 3 panels: left = tools, middle = analysis and data, and right = history and generated datasets" alt="Galaxy user interface showing the 3 panels: left = tools, middle = analysis and data, and right = history and generated datasets" width="100%" style="display: block; margin: auto;" />


Datasets for analysis in Galaxy can be **uploaded** from a laptop or desktop computer or obtained from public data repositories connected to Galaxy. With Galaxy, complex workflows composed of tens or even hundreds of analysis tools can be created and run. In Galaxy’s workflow interface, tools can be added and connected via a simple drag-and-drop approach. 

<img src="resources/images/05-Specific_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_141.png" title="Galaxy workflow example showing the beginning steps of a workflow" alt="Galaxy workflow example showing the beginning steps of a workflow" width="100%" style="display: block; margin: auto;" />


Galaxy users can share all their work—analysis histories, workflows, and visualizations—via simple URLs that are available to specific colleagues or a link that anyone can access. Galaxy’s user interface is highly scalable. Tens, hundreds, or even thousands of datasets can be grouped into collections and run in parallel using individual tools or multi-tool workflows. In summary, Galaxy is a popular computational workbench with tools and features for a wide variety of data analyses, and it has broad usage in cancer data analysis.


## SciServer

SciServer is similar to Galaxy in that it is accessible through a web browser and allows users to store, upload, download, share, and work with data and common tools on the same platform. It was originally built for the astrophysics community (and called SkyServer) but it has now been adapted to be used by scientists of all fields and is indeed used by many in the genomics field.  It allows users to use Python and R in environments like Jupyter notebooks and RStudio, and also supports (Structured Query Language) SQL for data querying and management and is built on the use of Docker. 

The main idea of SciServer, is based on this premise: "bring the analysis to the data". It is free to use after users register. However, users can buy extra resources. Users can keep data private or share their data. 

As compared to Galaxy, this resources may be better for users with a bit more familiarity with informatics but who require more flexibility, particularly for working with collaborators such as physicists or material scientists as there are more tools supported across disciplines. In addition it also gives users access to very large data sets on Petabyte-scale (note that some of these require special permission to use) and supports developers to create their own web interfaces called SciUIs for particular use cases.

For more information see 
https://reader.elsevier.com/reader/sd/pii/S2213133720300664?token=D3EB0851DC2A36526E6999F0D95DA1E6C41D01E9787B690B2F06F7CE7C192B7141B9FA6BAE5DF1D4BFAD7E402540624E&originRegion=us-east-1&originCreation=20211028203856

## Materials Cloud

https://www.nature.com/articles/s41597-020-00637-5

## AiiDA 
https://www.nature.com/articles/s41597-020-00638-4

## Atlas.ti?
https://atlasti.com/

I think featuring XNAT and OHIF open health imaging foundation might make sense... OHIF is an web-based imaging analysis platform that is widely used. It was developed by Gordon Harris et al.

https://www.toptal.com/scientific-computing/scientific-computing-with-open-source-tools

google: "https://www.youtube.com/embed/N4eT9Lfvuro"
