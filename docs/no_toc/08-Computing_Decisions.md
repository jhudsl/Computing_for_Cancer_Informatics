




# Data Management Decisions

In this chapter we will discuss aspects that you should consider when deciding what data and computing systems to use for your work. 


<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g115e0d5ae79_0_0.png" title="Learning Objectives: 1. Recognize the main aspects to focus on when deciding on what computing systems to use. 2. Be aware of the benefits and drawbacks of various options." alt="Learning Objectives: 1. Recognize the main aspects to focus on when deciding on what computing systems to use. 2. Be aware of the benefits and drawbacks of various options." width="100%" style="display: block; margin: auto;" />


To afford you the best opportunity to perform the informatics research that you would like, it is useful to become familiar with the benefits and drawbacks of various computing options. 


***Note:** This content was adapted from content by [Frederick Tan](https://leanpub.com/u/cutsort) for the [AnVIL project](https://anvilproject.org/). See his course created with [Jeff Leek](https://leanpub.com/u/jtleek), [Sarah Wheelan](https://leanpub.com/u/swheelan), and [Kai Kammers](https://leanpub.com/u/kaikammers)   [here](https://leanpub.com/universities/courses/jhu/anvil-intro).*





## Computing Platforms

Now that we have discussed a bit about how computers perform computations and computing options, lets discuss more about how you might choose your computing platform. A computing platform, is all the [hardware](https://simple.wikipedia.org/wiki/Computer_hardware) (the physical parts of your computing platform) and [software](https://simple.wikipedia.org/wiki/Software) (the code that tells the computing platform how to function) necessary to create the environment in which you can perform your computational work.

Choosing a computing platform involves both software and hardware decisions. 


## Choosing a Computing Platform

Choosing a [computing platform](https://en.wikipedia.org/wiki/Computing_platform) depends on several considerations.  

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g115e0d5ae79_0_5.png" title="General Considerations: 1. What type of interface is needed? 2. Will data need extra privacy protection? 3. How computationally intensive will the work be? 4.How much data storage is needed?" alt="General Considerations: 1. What type of interface is needed? 2. Will data need extra privacy protection? 3. How computationally intensive will the work be? 4.How much data storage is needed?" width="100%" style="display: block; margin: auto;" />


### General Considerations

Asking yourself and your research team these questions can help you find the right computing platform:

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


## Protected data

Are you working with protected data that requires special security precautions?

If you are working with data that might be protected by [HIPAA](https://www.hipaajournal.com/hipaa-compliance-checklist/), such as electronic health records, then special security measures are required to ensure that only authorized users have access to the data.

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g115e0d5ae79_0_43.png" title="HIPAA Logo" alt="HIPAA Logo" width="100%" style="display: block; margin: auto;" />

[[source](https://www.paubox.com/blog/what-is-hipaa/)]


### Computation needs

How computationally intensive are my tasks? 

If you have a large amount of data and/or are performing complex analyses, you may require more computational power than your current laptop can provide. If this is the case, you might consider using a local server or what is called "Cloud" computing (see the previous chapters for more info if you have not already). 



### Storage needs

How much storage space do I need for both temporary and long-term data?



## Local or Remote?

If you are working with large datasets you may also need storage options that go beyond what you currently have available. Local or "Cloud" storage options may work for you, depending on other considerations (security, data transfers) that we will discuss further. See  @fischer_jetstream_2019 for more information about the costs and benefits of using a cloud option like Jetstream for your computational work.


1) Are local resources sufficient? 

When a local solution already works, one may rightly question the time required to migrate to the Cloud.  However, when local solutions are insufficient or unsustainable, then the Cloud becomes a competitive option.

2) Do you work with especially big or controlled access datasets? 

Increasingly large datasets like the NCBI Sequence Read Archive are being stored on the Cloud.  If your work relies on being able to access the entire dataset, then the Cloud may be your only practical option.  Furthermore, if you work with controlled access data, then more platforms are providing compliance with regulations like HIPAA and FedRAMP.

3) Do you  need to work with collaborators?  Computational research increasingly involves larger and larger collaborations.  While many fragmented systems exist to share work, the Cloud presents an opportunity for everyone to share the exact same computational environment including hardware, software, and datasets.

If Cloud Computing makes sense for you, then you’re in luck!  The past decade has seen the development of many efforts to make Cloud computing, easier, faster, and more affordable.  As each platform has their strengths and weaknesses, we will now discuss several opportunities and challenges that Cloud computing presents in the field of computational genomics.

### Benefits of Cloud Computing

The state of Cloud computing is continually evolving.  Here, we highlight three main current benefits:


1) **Sharing Workflows**  

The first major benefit is the increasing ease with which one can share and collaborate on research projects. Shown here is the History feature of [Galaxy](https://usegalaxy.org/). Using this, one can share not only what datasets they used but also every computational manipulation that was performed.

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_38.png" title="Galaxy history example" alt="Galaxy history example" width="100%" style="display: block; margin: auto;" />


By sharing such a history, one can reproduce an analysis in its entirety (if they use the same data), allowing collaborators to offer comments and extend upon the work with ease.



2) **Sharing Workflows between Platforms**

While sharing complete analysis histories is for the most part constrained to a particular software platform, a second benefit that has arisen is the ability to share Workflows between platforms.

Shown here is a diagram of a single cell analysis pipeline published by the Klarman Cell Observatory on Dockstore:

<img src="resources/images/08-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_43.png" title="Workflow" alt="Workflow" width="100%" style="display: block; margin: auto;" />

This higher level abstraction coupled with container technology allows this multistep analysis to be run with relative ease on supporting platforms like Terra or DNAnexus.


3) **Using Commodity Hardware**

The third Benefit we highlight is the increasing ease by which one can provision commodity hardware at scale.  




What this means is that you can pay reasonable costs to complete your analysis in less time by renting hundreds to tens of thousands of Cloud-based computers -- importantly stopping the bill when your analysis is complete.  Specialized hardware like GPUs and large memory nodes are also available for rent allowing you to pay only for what you need.

### Challenges of Cloud Computing

Balancing these three benefits are four challenges:

1) **Data Transfer**  

Data transfer and data management remains a cumbersome task.  While storing data in the "Cloud" has its advantages, it also has corresponding storage costs. Thus, careful planning is necessary with regards to what data will be stored where, as well as budgeting the time necessary to transfer data back and forth.

2) **Data Security**  

Most Cloud resources offer features that make it easier to access and share data, and these features often come at the **expense of security**. Thus, special precautions must be implemented to securely store protected datasets such as human genome sequences and electronic health records.

3) **Costs** 

Controlling costs, especially with regards to storage, presents a third formidable challenge.  As many Cloud providers naturally want to encourage usage of their platforms, users must be aware of how much money is currently being spent and be able to project how much money is likely to be spent in the future.  We will briefly overview cost controls in the next section.

While software platforms can help mitigate these challenges, Cloud computing still incurs costs from the underlying hardware providers. 

4) **IT**  

A final challenge is that many IT support staff do not have extensive experience managing Cloud resources.  Should IT choose to support analysis on the Cloud, they would face the aforementioned challenges of understanding and supporting data management, security compliance, and cost management.  Fortunately, large initiatives like AnVIL, [Galaxy](https://usegalaxy.org/), and CyVerse continue to work on democratizing access to Cloud computing by tackling many of these challenges.  


## Conclusions


