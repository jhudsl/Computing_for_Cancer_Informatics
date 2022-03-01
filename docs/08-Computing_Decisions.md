




# Data Management Decisions

Now that we have discussed a bit about how computers perform computations and described a bit about computing options, lets discuss more about how you might choose the right computing resources for your work. In this chapter we will discuss aspects that you should consider when deciding between different computing resource options. 


<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g115e0d5ae79_0_0.png" title="Learning Objectives: 1. Recognize the main aspects to focus on when deciding on what computing systems to use. 2. Be aware of the benefits and drawbacks of various options. 3. Know what to watch out for in computing decisions." alt="Learning Objectives: 1. Recognize the main aspects to focus on when deciding on what computing systems to use. 2. Be aware of the benefits and drawbacks of various options. 3. Know what to watch out for in computing decisions." width="100%" style="display: block; margin: auto;" />


To afford you the best opportunity to perform the informatics research that you would like, it is useful to become familiar with the benefits and drawbacks of various computing options. First we will start out with some general considerations that you should think about when beginning to determine what computing option makes sense for your work.

The following are the major decision points for your computing needs:

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g1175806cc27_0_0.png" title="1. Personal vs Shared, 2. Local Shared vs Remote Shared 3. Which shared resource?" alt="1. Personal vs Shared, 2. Local Shared vs Remote Shared 3. Which shared resource?" width="100%" style="display: block; margin: auto;" />


***Note:** This content was adapted from content by [Frederick Tan](https://leanpub.com/u/cutsort) for the [AnVIL project](https://anvilproject.org/). See his course created with [Jeff Leek](https://leanpub.com/u/jtleek), [Sarah Wheelan](https://leanpub.com/u/swheelan), and [Kai Kammers](https://leanpub.com/u/kaikammers)   [here](https://leanpub.com/universities/courses/jhu/anvil-intro).*


## General Computing Considerations

Choosing a [computing platform](https://en.wikipedia.org/wiki/Computing_platform) depends on several considerations.  

Asking yourself and your research team the following questions can help you find the right computing platform.

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g115e0d5ae79_0_5.png" title="General Considerations: 1. How computationally intensive will the work be? 2. How much data storage is and will be needed? 3. Do I plan on collaborating with others outside my institute? 4. Does my data that need extra privacy protection? 5. How much money can I spend on computing? 6. Do I want extra guidance for my informatics work? 7. Do I need flexibility? Might I work with more data modalities in the future? 8. Do I need scalability? Will I soon work with more data? 9. Do I need access to large controlled datasets? 10.What kind of interface would be helpful?" alt="General Considerations: 1. How computationally intensive will the work be? 2. How much data storage is and will be needed? 3. Do I plan on collaborating with others outside my institute? 4. Does my data that need extra privacy protection? 5. How much money can I spend on computing? 6. Do I want extra guidance for my informatics work? 7. Do I need flexibility? Might I work with more data modalities in the future? 8. Do I need scalability? Will I soon work with more data? 9. Do I need access to large controlled datasets? 10.What kind of interface would be helpful?" width="100%" style="display: block; margin: auto;" />

Let's take a bit of a deeper dive now for each of these considerations.

### Computation needs

Now that you know more about determining your personal computer's computing and storage capacity, as well as how to determine or estimate the files sizes that you might use for your research, you can begin to assess if your personal computer is up to the task. When determining what your computing needs might be, remember to evaluate how many files you might use in your analyses, the file sizes, the amount of RAM and CPUs (and possibly GPUs that your computer has) and some level of understanding for how intensive the computing tasks are that you plan to perform. How do you assess this?  If the files that you intend to use in your analysis are quite large for your computer's storage capacity, then it is likely that your computer might struggle to work with such files. This might also be the case if you plan to use many many smaller files. Finally, if you plan to perform many steps on your files in your analysis this may also require more computing resources than you have available on your current personal computer. Shared computing options will generally have the capacity to allow you to do your work, unless you have very large data needs and you hope to use a very specialized computing platform that may not support large-scale work. Checking with the local or remote computing options that you are interested in about the computing capacity ahead of time before you start an analysis if you have large data analysis plans would be a good idea.

### Data storage

Again, now that you know how to assess the data storage potential of your computer, you can decide if your computer can handle storing all the files that you might wish to use in your analysis. Think about your current data analysis plans but keep in mind your future plans as well. If you hope to replicate experiments with more samples, you might run out of storage. One way around this is to by external additional storage (which is also a good idea for backing up your data!). However, if you think that you might have much larger scale research plans in the future, you might want to think about shared computing options. Cloud computing platforms and more traditional servers have different storage capacities, so it is worth checking out the options that might be helpful for your research. Also keep in mind that it will take time to transfer your data, especially if your data is very large.

### Multi-institute collaboration

If you plan to work with others outside of your institute that would not have access to the same local shared computing resources, then remote computing options would be really helpful for allowing your collaborators to work on the same data together. Cloud platforms especially make it easier for collaboration, as everyone can share the exact same computational environment including hardware, software, and datasets.

### Protected data

Are you working with protected data that requires special security precautions?

If you are working with data that might be protected by [HIPAA](https://www.hipaajournal.com/hipaa-compliance-checklist/), such as electronic health records, then special security measures are required to ensure that only authorized users have access to the data. Be careful about both traditional shared and cloud computing resources. Sometimes extra privacy and data security measures are built in and at other times, you will need perform extra steps to get the data security and privacy that you need. Although many cloud computing systems do not allow for extra privacy, there are platforms that provide compliance with regulations like [HIPAA](https://www.hipaajournal.com/hipaa-compliance-checklist/) and [FedRAMP](https://blog.hootsuite.com/what-is-fedramp/).

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g115e0d5ae79_0_43.png" title="HIPAA Logo" alt="HIPAA Logo" width="100%" style="display: block; margin: auto;" />

[[source](https://www.paubox.com/blog/what-is-hipaa/)]



### Costs

Often local shared computing resources at your institute can be much less expensive than some of the common cloud computing options. However, this is not always the case and if you have very specific analysis goals in mind, the benefit of cloud computing resources, is that you typically only pay for the resources that you actually use. This does also involves learning how costs are calculated for the particular cloud resource, which can be a challenge, but many cloud platforms that were designed for research such as [Jetstream](https://jetstream-cloud.org/) or [Terra/AnVIL](https://support.terra.bio/hc/en-us/articles/360029772212-Controlling-Cloud-costs-sample-use-cases) can be very affordable and in some cases some small platforms offer free resources.  

### Extra guidance

Cloud computing platforms such as [Galaxy](https://galaxyproject.org/), [AnVIL](https://support.terra.bio/hc/en-us/articles/360029772212-Controlling-Cloud-costs-sample-use-cases), and [GenePattern](https://www.genepattern.org/) offer lots of training material and resources about how to actually perform analyses, especially for genomic analyses. Galaxy also supports other types of data, as do many other platforms, as described in the last chapter. Having the extra guidance like that offered with these types of platforms can be very beneficial to investigators that are trying out new methods!

### Flexibility

If you plan on working with multiple data modalities like for example both imaging and genomic data, consider computing options that are flexible for such analyses. Some cloud computing options designed for research are more general and supportive of this, such as [Galaxy](https://galaxyproject.org/) to some extent, as well as to a larger extent [SciServer](https://jhudatascience.org/Computing_for_Cancer_Informatics/research-platforms.html), [Jetstream](https://jetstream-cloud.org/), or [CyVerse](https://cyverse.rocks/about).


### Scalability

If you hope to start using very large datasets or plan to collaborate with many people using many different data sets, then you might need to keep in mind the future storage and computing capacity of the computing resources that you are considering. Starting with an option that allows for much more data storage and computing such as many of the more general cloud computing options might be best for you in this case, as you might find yourself restricted by smaller cloud platforms or more traditional shared computing resources.

### Data access

Some cloud computing options already have data available that may be of interest for you and your work. For example [Galaxy](https://galaxyproject.org/), [AnVIL](https://support.terra.bio/hc/en-us/articles/360029772212-Controlling-Cloud-costs-sample-use-cases), and [GenePattern](https://www.genepattern.org/) provide access to many genomic datasets. Smaller platforms can also have access to data that may be of specific more clinical interest to you as well such as the [Cancer Genome Collaboratory](https://cancercollaboratory.org/), which provides access to data from the [International Cancer Genome Consortium (ICGC)](https://en.wikipedia.org/wiki/International_Cancer_Genome_Consortium). 

### Interface

Will you need a [graphical interface](https://www.omnisci.com/technical-glossary/graphical-user-interface), a [command line interface](https://searchwindowsserver.techtarget.com/definition/command-line-interface-CLI), or both?

What do we mean by this?

A [graphical user interface](https://www.omnisci.com/technical-glossary/graphical-user-interface) or simply just graphical interface or GUI, allows for users to choose functions to perform by interacting with visual representations. They have a "user-centered" design that creates a visual environment where users can for example **click on** tabs, boxes, or icons for to perform functions. This also often allows users to more directly see plots and other types of visualizations.

[Galaxy](https://usegalaxy.org/) offers a graphical user interface for performing analyses and tasks. For example in the following image we show a GUI for joining two files:

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_33.png" title="Galaxy Graphical User Interface" alt="Galaxy Graphical User Interface" width="100%" style="display: block; margin: auto;" />


Another Graphical User Interface example comes from the [OHIF image viewer](https://ohif.org) which has a tool bar for modifying, viewing and annotating images.

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfd8d3f477a_159_2.png" title="The OHIF Graphical User Interface has an image viewer (center) which  includes a tool bar (above center) to modify, view, and annotate images. A menu on the left allows users to access images related to the current patient in other studies, and a menu on the right is used for making measurements and exporting measurement reports." alt="The OHIF Graphical User Interface has an image viewer (center) which  includes a tool bar (above center) to modify, view, and annotate images. A menu on the left allows users to access images related to the current patient in other studies, and a menu on the right is used for making measurements and exporting measurement reports." width="100%" style="display: block; margin: auto;" />


A [command line interface](https://searchwindowsserver.techtarget.com/definition/command-line-interface-CLI) (also known as a character interface) allows for software functions to be performed by specifying through commands written in text. This typically offers more control than a graphical interface, however command line interfaces are often less user friendly as they require that the user know the correct commands to use.

For example, one could perform functions in R using Bioconductor packages such as [Biostrings](https://bioconductor.org/packages/release/bioc/html/Biostrings.html) with a command line interface:

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g115e0d5ae79_0_35.png" title="Command line interface using R and Bioconductor package" alt="Command line interface using R and Bioconductor package" width="100%" style="display: block; margin: auto;" />



A situation where you might use **both** a command line interface and a GUI, is using [RStudio](https://en.wikipedia.org/wiki/RStudio) to perform an analysis in R with Bioconductor packages. [RStudio](https://en.wikipedia.org/wiki/RStudio) is what is called an IDE or an [integrated development environment](https://en.wikipedia.org/wiki/Integrated_development_environment), which is an application that supports writing code. There are many tools to help you including a console for writing code in R with command line interfacing, as well as graphical interface tools. As shown in this example below, one can inspect and save a plot (that was created with the command line) by using a GUI. The plot was created using the same package as the one used in the command line interface example.

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g115e0d5ae79_0_30.png" title="Command line interface using R and Bioconductor package with a GUI using RStudio" alt="Command line interface using R and Bioconductor package with a GUI using RStudio" width="100%" style="display: block; margin: auto;" />

Some cloud computing options will have either interface option while others will only have one. This is an important consideration when you decide what computing resources to use.

## Local shared resources vs remote shared resources

Often the first decision about cloud computing resources is based on determining if your personal computer can handle your work. If you have already determined that you indeed need more computing power than your personal lab computers, the next decision is between local shared resources and more traditional shared resources, like XSEDE, and cloud computing options. See  @fischer_jetstream_2019 for more information about the costs and benefits of using a cloud option like Jetstream for your computational work. We will now discuss some questions that you might ask yourself to make the decision between local and remote shared computing resources.


1) Are local shared computing resources sufficient? 

When a local computing resource solution already works, one may rightly question the time required to learning how to use a new cloud-based platform. However, when local solutions are insufficient or unsustainable (say other users often use up most of the resources or a server is often down), then the cloud becomes a competitive option.

2) Do you want to work with especially big or controlled access datasets? 

Increasingly large datasets like the [Genotype -Tissue Expression (GTEx)](https://gtexportal.org/home/), [Therapeutically Applicable Research to Generate Effective Treatments (TARGET)](https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/study.cgi?study_id=phs000218.v24.p8) or [The Cancer Genome Atlas (TCGA)](https://www.cancer.gov/about-nci/organization/ccg/research/structural-genomics/tcga) are being stored on the cloud-based platforms. If your work relies on being able to access a large dataset like this, then the cloud may be your only practical option. 

3) Do you need to work with collaborators?  Computational research increasingly involves larger and larger collaborations. While many systems exist to share work,  cloud platforms make it easier for everyone to share the exact same computational environment including hardware, software, and datasets.

We will now discuss several opportunities and challenges that cloud computing currently presents.

### Benefits of Cloud Computing

The state of Cloud computing is continually evolving.  Here, we highlight the main current benefits:


1) **Sharing history**  

The first major benefit is the increasing ease with which one can share and collaborate on research projects. Shown here is the History feature of [Galaxy](https://usegalaxy.org/). Using this, one can share not only what datasets they used but also every computational manipulation that was performed.

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_38.png" title="Galaxy history example" alt="Galaxy history example" width="100%" style="display: block; margin: auto;" />


By sharing such a history, one can reproduce an analysis in its entirety (if they use the same data), allowing collaborators to offer comments and extend upon the work with ease.



2) **Sharing Workflows between Platforms**

While sharing complete analysis histories is for the most part constrained to a particular software platform, a second benefit that has arisen is the ability to share workflows between platforms.[Dockstore](https://dockstore.org/) is a great open-source and free option to share and find bioinformatics workflows that can be launched using different platforms.

Shown here is a diagram of an analysis pipeline to create a [custom reference](https://support.10xgenomics.com/single-cell-gene-expression/software/pipelines/latest/advanced/references) for single cell 10x data using [cell ranger](https://support.10xgenomics.com/single-cell-gene-expression/software/pipelines/latest/what-is-cell-ranger) published by the Klarman Cell Observatory on [Dockstore](https://dockstore.org/workflows/github.com/klarman-cell-observatory/cumulus/Cellranger_create_reference:master?tab=dag). Users can launch the workflow on various supported platforms such as Terra or AnVIL.:

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g117032ee319_0_8.png" title="Workflow on Dockstore showing launch buttons with multiple platforms" alt="Workflow on Dockstore showing launch buttons with multiple platforms" width="100%" style="display: block; margin: auto;" />

This higher level abstraction coupled with container technology allows this multistep analysis to be run with relative ease on supporting platforms like Terra, AnVIL, or [DNAnexus](https://www.dnanexus.com/), which is yet another computing platform company, although with generally more costs associated as compared to Terra or AnVIL.


3) **Using Commodity Hardware**

The third Benefit we highlight is the increasing ease by which one can provision commodity hardware at scale.  

What this means is that you can pay reasonable costs to complete your analysis in less time by renting hundreds to tens of thousands of Cloud-based computers -- importantly stopping the bill when your analysis is complete.  Specialized hardware like GPUs and large memory nodes are also available for rent allowing you to pay only for what you need.

4) **Less Etiquette**

Relative to more traditional shared computing resources, you don't need to worry as much about sharing etiquette with cloud computing options because these resources typically have more than enough to go around. There is a trade off in that you will need to learn how to work with the cloud computing platform, however you can be more independent about what software you use and how many resources you use without bothering others.

5) **Data Access**

Easy access to large datasets that might be otherwise difficult to work with. Now many cloud computing resources, especially those designed for research, also allow users access to relevant datasets. 

### Challenges of Cloud Computing

Balancing these benefits are the following challenges:

1) **Data Transfer**  

Data transfer and data management remains a cumbersome task.  While storing data in the cloud has its advantages, it also has corresponding storage costs. Thus, careful planning is necessary with regards to what data will be stored where, as well as budgeting the time necessary to transfer data back and forth. However if you have yet to start work on a local shared computing resource than the work to transfer may be comparable. Additionally if you plan to use public data that is accessible through a platform designed for research than you may in fact have less data transfer needs when working with a cloud computing option. 

2) **Data Security**  

Most cloud resources offer features that make it easier to access and share data, and these features often come at the **expense of security**. Thus, special precautions must be implemented to securely store protected datasets such as human genome sequences and electronic health records. 

Some of the specialized research platforms allow for this as described in the previous chapter. Make sure you check what is required to set up an extra security protection - often this will not be automatic. Also keep in mind that although local shared resources like that of your university often have good security and data privacy policies and protection mechanisms, this is not always the case.

3) **Costs** 

Controlling costs, especially with regards to storage, presents a third formidable challenge.  As many cloud providers naturally want to encourage usage of their platforms, users must be aware of how much money is currently being spent and be able to project how much money is likely to be spent in the future.  

While software platforms can help mitigate these challenges, cloud computing still incurs costs from the underlying hardware providers. It can be a challenge to understand how this is billed.

4) **IT**  

A final challenge is that many IT support staff do not have extensive experience managing cloud resources.  Should IT choose to support analysis on the cloud, they would face the aforementioned challenges of understanding and supporting data management, security compliance, and cost management.  Fortunately, large initiatives like AnVIL, [Galaxy](https://usegalaxy.org/), and CyVerse continue to work on democratizing access to cloud computing by tackling many of these challenges.  


## Choosing between remote sharing options

The final major decision, should you decide that you want to go with a remote sharing option is to decide which remote computing resource to go with. 

This decision should be based on the following:

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g1175806cc27_0_27.png" title="1) Does the resource offer the privacy protection needed? 2) Does the resource allow for me to use the data modalities I need? 3) Does the resource already have data that I might want? 4) Does the resource provide extra guidance that might be helpful for my work? 5) Does the resource offer the interface that I would like to work with? 6) Does the resource offer me access to a relevant community for my work that would be helpful?" alt="1) Does the resource offer the privacy protection needed? 2) Does the resource allow for me to use the data modalities I need? 3) Does the resource already have data that I might want? 4) Does the resource provide extra guidance that might be helpful for my work? 5) Does the resource offer the interface that I would like to work with? 6) Does the resource offer me access to a relevant community for my work that would be helpful?" width="100%" style="display: block; margin: auto;" />






## Overall Decision Process

We suggest evaluating your computing needs based on the following decision tree.

<div id="C660C4AD4516EA9D6EEABE9A9B7980244BE_91242"><div id="C660C4AD4516EA9D6EEABE9A9B7980244BE_91242_robot"><a href="https://cloud.smartdraw.com/share.aspx/?pubDocShare=C660C4AD4516EA9D6EEABE9A9B7980244BE" target="_blank"><img src="https://cloud.smartdraw.com/cloudstorage/C660C4AD4516EA9D6EEABE9A9B7980244BE/preview2.png"></a></div></div><script src="https://cloud.smartdraw.com/plugins/html/js/sdjswidget_html.js" type="text/javascript"></script><script type="text/javascript">SDJS_Widget("C660C4AD4516EA9D6EEABE9A9B7980244BE",91242,0,"");</script><br/>

Or click on this link: https://cloud.smartdraw.com/share.aspx/?pubDocShare=C660C4AD4516EA9D6EEABE9A9B7980244BE

<iframe src="https://cloud.smartdraw.com/share.aspx/?pubDocShare=C660C4AD4516EA9D6EEABE9A9B7980244BE" width="100%" height="400px"></iframe>

## Conclusions

We hope that this chapter has given you some more perspective on how to make important computing decisions to make the most out of your work.

In conclusion, here are some of the major take-home messages:

1) The three major computing decisions are: 1. Personal computer vs Shared resource, 2. Local shared resource vs. Remote Shared resource, 3. Which shared resource. Start first with determining if your personal computer can handle your work or if you have plans to collaborate with others at different institutes.

2) The following are general considerations that can help you make each of the 3 decisions: 1. How computationally intensive will the work be? 2. How much data storage is and will be needed? 3. Do I plan on collaborating with others outside my institute? 4. Does my data that need extra privacy protection? 5. How much money can I spend on computing? 6. Do I want extra guidance for my informatics work? 7. Do I need flexibility? Might I work with more data modalities in the future? 8. Do I need scalability? Will I soon work with more data? 9. Do I need access to large controlled datasets? 10. What kind of interface would be helpful? 

3) The main benefits of cloud options are easier sharing of data, code, and workflows even across different computing platforms, access to large amounts of computing resources, generally only need to pay for the resource you actually use, less need to be as conscious of proper etiquette for sharing computing resources.

4) The main drawbacks of cloud options in general are: 1. if you were already using a shared resource then migrating to the cloud will require data transfer effort and time, 2. Some cloud computing options do not provide data privacy protection that may be needed for certain types of data, 3. costs calculations can be especially confusing and you will need to learn how it works for the particular resource that you are interested in using, 4. There will be less IT support form your local IT department as many of these resources have their own infrastructure, however many options provide their own guidance and support.


3) More and more cloud computing options are being developed and designed specifically for research, consider the following questions when choosing between cloud-based options: 1. Does the resource offer the privacy protection needed? 2. Does the resource allow for me to use the data modalities I need? 3. Does the resource already have data that I might want? 4. Does the resource provide extra guidance that might be helpful for my work? 5. Does the resource offer the interface that I would like to work with? 6. Does the resource offer me access to a relevant community for my work that would be helpful?

