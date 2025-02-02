



# General Platforms

In this chapter we will provide examples of computing systems that you might find useful for your research. Please note that we aim to provide a general overview of options and thus this is not a complete list. Let us know if there is a platform or system that you think we should include!

<img src="resources/images/06-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf5f8818810_1_171.png" title="Learning Objectives: 1.Recognize general informatics computing and data management platforms. 2.Be aware of specific genomics data management systems 3.Be aware of specific imaging data management systems  4.Be aware of specific clinical data management systems" alt="Learning Objectives: 1.Recognize general informatics computing and data management platforms. 2.Be aware of specific genomics data management systems 3.Be aware of specific imaging data management systems  4.Be aware of specific clinical data management systems" width="100%" style="display: block; margin: auto;" />

avocado:https://go.cloudhealthtech.com/eb-simplify-the-journey-data-center-to-public-cloud.html

We will start out with more general computing platforms, that allow you flexibility to perform analyses with a variety of types of data. The major advantage of these platforms is that users can analyze data where it lives. There is less need for data transfers, saving time an resources, and users can easily share data with the entire field. 

### Galaxy

This section was written by [Jeremy Goecks](https://goeckslab.org/people/jeremy.html):

Galaxy is a web-based computational workbench that connects analysis tools, biomedical datasets, computing resources, a graphical user interface, and a programmatic API. Galaxy (https://galaxyproject.org/) enables accessible, reproducible, and collaborative biomedical data science by anyone regardless of their informatics expertise. There are more than 8,000 analysis tools and 200 visualizations integrated into Galaxy that can be used to process a wide variety of biomedical datasets. This includes tools for analyzing genomic, transcriptomic (RNA-seq), proteomic, metabolomic, microbiome, and imaging datasets, tool suites for single-cell omics and machine learning, and thousands of more tools. Galaxy’s graphical user interface can be used with only a web browser, and there is a programmatic API for performing scripted and automated analyses with Galaxy.

<img src="resources/images/06-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_131.png" title="Galaxy can be accessed through a web browser and provides users with access to tools, datasets, computing resources, a graphical user interface (GUI) for users who would like to interact with Galaxy by clicking buttons and using drop-down menus and a programmtic API for users that would like to write code to interact with Galaxy" alt="Galaxy can be accessed through a web browser and provides users with access to tools, datasets, computing resources, a graphical user interface (GUI) for users who would like to interact with Galaxy by clicking buttons and using drop-down menus and a programmtic API for users that would like to write code to interact with Galaxy" width="100%" style="display: block; margin: auto;" />

Galaxy is used daily by thousands of scientists across the world. A vibrant Galaxy community has deployed hundreds of Galaxy servers across the world, including more than 150 public and three large national/international servers in the United States, Europe, and Australia (https://usegalaxy.org, https://usegalaxy.eu, https://usegalaxy.org.au). The three national/international servers have more than 250,000 registered users who execute >500,000 analysis jobs each month. Galaxy has been cited more than 10,000 times with >20% from papers related to cancer. The Galaxy Tool Shed (https://usegalaxy.org/toolshed) provides a central location where developers can upload tools and visualizations and users can search and install tools and visualizations into any Galaxy server. Galaxy has a large presence in the cancer research community. Galaxy serves as an integration and/or analysis platform for 7 projects in the NCI ITCR program. There is also increasing use of Galaxy in key NIH initiatives such as the NCI Cancer Moonshot Human Tumor Atlas Network (HTAN) and the NHGRI Data Commons, called the AnVIL (https://anvilproject.org/).

<img src="resources/images/06-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_135.png" title="Map of the 3 Galaxy servers" alt="Map of the 3 Galaxy servers" width="100%" style="display: block; margin: auto;" />


Galaxy’s user interface, accessible via a web browser, provides access to all Galaxy functionality. The main Galaxy interface has three panels: available tools (left), running analyses and viewing data (middle), and a full history of tools run and datasets generated (right). 

<img src="resources/images/06-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_111.png" title="Galaxy user interface showing the 3 panels: left = tools, middle = analysis and data, and right = history and generated datasets" alt="Galaxy user interface showing the 3 panels: left = tools, middle = analysis and data, and right = history and generated datasets" width="100%" style="display: block; margin: auto;" />


Datasets for analysis in Galaxy can be **uploaded** from a laptop or desktop computer or obtained from public data repositories connected to Galaxy. With Galaxy, complex workflows composed of tens or even hundreds of analysis tools can be created and run. In Galaxy’s workflow interface, tools can be added and connected via a simple drag-and-drop approach. 

<img src="resources/images/06-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_141.png" title="Galaxy workflow example showing the beginning steps of a workflow" alt="Galaxy workflow example showing the beginning steps of a workflow" width="100%" style="display: block; margin: auto;" />


Galaxy users can share all their work—analysis histories, workflows, and visualizations—via simple URLs that are available to specific colleagues or a link that anyone can access. Galaxy’s user interface is highly scalable. Tens, hundreds, or even thousands of datasets can be grouped into collections and run in parallel using individual tools or multi-tool workflows. In summary, Galaxy is a popular computational workbench with tools and features for a wide variety of data analyses, and it has broad usage in cancer data analysis.

See[here](https://toolshed.g2.bx.psu.edu/) for the list of applications supported by Galaxy.





### Terra

[Terra](https://terra.bio/) is a biomedical research computing platform that is based on the Google Cloud platform, that also allows users easier ways to manage the billing of their projects. It provides users with access to data, workflows, interactive analyses using Jupyter Notebooks, RStudio, and Galaxy, data access tools from [FireCloud from the Broad Institute](https://firecloud.terra.bio/) (a [National Cancer Institute (NCI)](https://www.cancer.gov/) Cloud Resource project),  as well as workspaces to organize projects and collaborate with others. Terra also has [many measures](https://terra.bio/resources/security/) to ensure that data is especially secure and the offer clinical features for ensuring that [health data is protected](https://terra.bio/about/privacy/). Note that according users who do upload protected health information must select to use these extra clinical features and enter a formal agree with [FireCloud](https://firecloud.terra.bio/) about their data. 

Importantly users can get access to use [Genotype -Tissue Expression (GTEx)](https://gtexportal.org/home/), [Therapeutically Applicable Research to Generate Effective Treatments (TARGET)](https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/study.cgi?study_id=phs000218.v24.p8) and [The Cancer Genome Atlas (TCGA)](https://www.cancer.gov/about-nci/organization/ccg/research/structural-genomics/tcga) data using the platform. See [here](https://support.terra.bio/hc/en-us/articles/4402326091675-Accessing-GTEx-TARGET-TCGA-data) for information on how. 

Users can pay for data storage and computing costs for Google Cloud conveniently through Terra. users can browse data for free.

Check out this video for more information:

<iframe src="https://www.youtube.com/embed/3rH86vcAqK8" width="100%" height="400px"></iframe>


## FireCloud

Users can also specifically use [FireCloud](https://datacommons.cancer.gov/analytical-resource/broad-institute-firecloud) as a data analysis platform which uses Terra, much like Terra uses FireCloud for various features. At this [link](https://support.terra.bio/hc/en-us/articles/360022694271) you can see a comparison of the two. 

FireCloud which is a project from the Broad institute and funded by the [National Institutes of Health (NIH)](https://www.nihlibrary.nih.gov/training/introduction-broad-firecloud-powered-terra-securely-analyzing-cancer-datasets-cloud). Datasets accessible to Terra are also accessible through FireCloud.

## AnVIL

If you could use some guidance on how to perform analyses using Galaxy and Terra, especially for genomic research, check out [AnVIL](https://anvilproject.org/), the [National Human Genome Research Institute (NHGRI)](https://www.genome.gov/) Analysis Visualization and Informatics Lab-space. It also provides access to many important genomic and related [datasets](https://anvilproject.org/data) from the NHGRI.


According to their website:

> By providing a unified environment for data management and compute, AnVIL eliminates the need for data movement, allows for active threat detection and monitoring, and provides elastic, shared computing resources that can be acquired by researchers as needed.

It relies on Terra for the cloud based compute environment, Dockstore for  standardized tools and workflows, Gen3 for data management for querying and organizing data, Galaxy tools and environment for analyses with less code requirements, and Bioconductor tools for R programming users.


### CyVerse

[CyVerse](https://cyverse.rocks/about) is a computing platform or cyberinfastructure similar to Galaxy that also offers computing resources for storing, sharing, and working with data with a graphical interface, as well as an API. Computing was previously offered using the cloud computing platform from CyVerse called [Atmosphere](https://cyverse.org/refocusing-atmosphere-to-support-cloud-native-development), which relied on users using virtual machines. Users will now  use a new version of Atmosphere with partnership with [Jetstream](https://jetstream-cloud.org/). This allows users to use containers for easier collaboration and also offers US users more computing power and storage. Originally called iPlant Collaborative, it was started by a funding from the National Science Foundation (NSF) to support life sciences research, particularly to support ecology, biodiversity, sustainability, and agriculture research. It is led by the University of Arizona, the Texas Advanced Computing Center, and Cold Spring Harbor Laboratory. It offers access to an environment for performing analyses with Jupyter (for Python mostly) and RStudio (for R mostly) and a variety of tools for Genomic data analysis. See [here](https://cyverse.atlassian.net/wiki/spaces/DEapps/pages/241882146/List+of+Applications) for a list of applications that are supported by CyVerse.  Note that you can also install tools on both platforms. Both CyVerse and Galaxy offer lots of helpful documentation, to help users get started with informatics analyses.

See [here](https://learning.cyverse.org/en/latest/) to learn more.

<img src="resources/images/06-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfd56752f25_0_0.png" title="CyVerse graphical interface for performing analyses" alt="CyVerse graphical interface for performing analyses" width="100%" style="display: block; margin: auto;" />

### SciServer

SciServer is similar to Galaxy in that it is accessible through a web browser and allows users to store, upload, download, share, and work with data and common tools on the same platform. It was originally built for the astrophysics community (and called SkyServer) but it has now been adapted to be used by scientists of all fields and is indeed used by many in the genomics field.  It allows users to use Python and R in environments like Jupyter notebooks and RStudio, and also supports (Structured Query Language) SQL for data querying and management and is built on the use of Docker. 

The main idea of SciServer, is based on this premise: "bring the analysis to the data". It is free to use after users register. However, users can buy extra resources. Users can keep data private or share their data. 

As compared to Galaxy, this resources may be better for users with a bit more familiarity with informatics but who require more flexibility, particularly for working with collaborators such as physicists or material scientists as there are more tools supported across disciplines. In addition it also gives users access to very large data sets on Petabyte-scale (note that some of these require special permission to use) and supports developers to create their own web interfaces called SciUIs for particular use cases.

For more information see 
https://reader.elsevier.com/reader/sd/pii/S2213133720300664?token=D3EB0851DC2A36526E6999F0D95DA1E6C41D01E9787B690B2F06F7CE7C192B7141B9FA6BAE5DF1D4BFAD7E402540624E&originRegion=us-east-1&originCreation=20211028203856


<img src="resources/images/06-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfd56752f25_0_13.png" title="The SciServer dashboard allows users to interact with the various resources and tools available through SciServer. Most are available through the command line but some have user interface options. Jupyter Notebooks, RStudio and SciUIs (interfaces created by other SciServer users) can be used to interactively explore and analyze data by users." alt="The SciServer dashboard allows users to interact with the various resources and tools available through SciServer. Most are available through the command line but some have user interface options. Jupyter Notebooks, RStudio and SciUIs (interfaces created by other SciServer users) can be used to interactively explore and analyze data by users." width="100%" style="display: block; margin: auto;" />



### Materials Cloud

Another resource that might be of interest to Python users, particular those who collaborate with material scientists, is Materials Cloud. It is designed to promote reproducible work, collaboration, and sharing of resources among scientists, particularly for simulations for the materials science field. Users can share data in a citable way, download data, upload data, share workflows, and perform analyzes.

<img src="resources/images/06-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfd56752f25_0_6.png" title="Materials Cloud resources are based on allowing users to Learn about resources, Work using the resources, Discover aspects about data that is available, Explore data with interactive graphs, and archive to store and share data." alt="Materials Cloud resources are based on allowing users to Learn about resources, Work using the resources, Discover aspects about data that is available, Explore data with interactive graphs, and archive to store and share data." width="100%" style="display: block; margin: auto;" />

This resource uses [AiiDAlab](https://www.materialscloud.org/work/aiidalab) as the computing environment for researchers, which is based on [AiiDA](https://www.nature.com/articles/s41597-020-00638-4). According to their website:

> AiiDAlab builds on [AiiDA](https://www.nature.com/articles/s41597-020-00638-4) as the computational workflow engine, and the Jupyter environment (notebooks, widgets, …) for writing and sharing apps

See [here](https://www.sciencedirect.com/science/article/pii/S092702562030656X?via%3Dihub) to learn more about how AiiDAlab supports the sharing of scientific workflows, particularly for those that use Python.

To learn more about Materials Cloud, check out this [article](https://www.nature.com/articles/s41597-020-00637-5)


### ATLAS.ti

[ATLAS.ti](https://atlasti.com/) is another option but particularly for qualitative analysis. You can use a variety of data types including video, audio, images, surveys, and social media data. A variety of tools, particularly for text data analysis are provided for methods such as [sentiment analysis](https://en.wikipedia.org/wiki/Sentiment_analysis), which is the process of assigning a general tone or feeling to text and [named-entity recognition](https://en.wikipedia.org/wiki/Named-entity_recognition), which is the process of extracting certain characteristics from texts that are what is called a [named entity] or a real-world object - such as a person's name or address. Such analyses can be helpful for understanding behaviors that might be associated with cancer risk. Although this type of analysis can be performed using R or Python among other coding languages, ATLAS.ti offers a nice graphical user interface to perform these types of analyses s.Furthermore ATLAS.ti offers a great deal of flexibility about such analyses using different data types easily.

<iframe src="https://downloads.atlasti.com/docs/branding/atlasti_brochure_v9_EN_interactive_202110.pdf" width="672" height="400px"></iframe>

## WebMeV
https://webmev.tm4.org/#/about

## Overture
https://dcc.icgc.org/

Avocado - want to add in content about price, security, privacy/HIPAA, scalability/file/ram limits for each if possible as table


