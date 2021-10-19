---
title: "Data Management Decisions"
output: html_document
---




# Data Management Decisions

In this chapter we will discuss aspects that you should consider when deciding what data and computing management systems to use for your own work. 

<img src="resources/images/05-Computing_Decisions_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf5f8818810_1_171.png" title="Learning Objectives: 1.Recognize general informatics computing and data management platforms. 2.Be aware of specific genomics data management systems 3.Be aware of specific imaging data management systems  4.Be aware of specific clinical data management systems" alt="Learning Objectives: 1.Recognize general informatics computing and data management platforms. 2.Be aware of specific genomics data management systems 3.Be aware of specific imaging data management systems  4.Be aware of specific clinical data management systems" width="100%" style="display: block; margin: auto;" />


To afford you the best opportunity to perform the informatics research that you would like, it is useful to become familiar with computing options and costs. This course aims to provide research leaders with some guidance about making decisions for computing [hardware](https://simple.wikipedia.org/wiki/Computer_hardware) (the physical parts of your computing platform) and [software](https://simple.wikipedia.org/wiki/Software) (the code that tells the computing platform how to function). It will also describe the benefits and drawbacks of local and "Cloud" computing, as well as the associated costs of each.

***Note:** This content was adapted from content by [Frederick Tan](https://leanpub.com/u/cutsort) for the [AnVIL project](https://anvilproject.org/). See his course created with [Jeff Leek](https://leanpub.com/u/jtleek), [Sarah Wheelan](https://leanpub.com/u/swheelan), and [Kai Kammers](https://leanpub.com/u/kaikammers)   [here](https://leanpub.com/universities/courses/jhu/anvil-intro).*





## Computing Platforms

Now that we have discussed a bit about how computers perform computations, lets discuss more about how you might choose your computing platform. A computing platform, is all the [hardware](https://simple.wikipedia.org/wiki/Computer_hardware) (the physical parts of your computing platform) and [software](https://simple.wikipedia.org/wiki/Software) (the code that tells the computing platform how to function) necessary to create the environment in which you can perform your computational work.

Choosing a computing platform involves both software and hardware decisions. We will focus on hardware.

## Hardware

With regards to hardware, there are two major options:  

1) Personal computers   
2) Shared computers   




### **Personal computers**

These are computers that your lab might own, such as a laptop, a desktop, or a small [server](https://techterms.com/definition/server) used by just your lab.  





![](images/Personal.png)
If you are not performing intensive computational tasks, it is possible that you will only need personal computers for your lab. However, you may find that this changes, and you might require connecting your personal computers to shared computers for more computational power and or storage.

Note that you could technically purchase your own server. However, this is very likely not as economical, feasible (as having your own server would require that you personally maintain it), or scalable (you might outgrow your server) as other computing options that we will discuss in a bit. 


https://profs.info.uaic.ro/~adria/teach/courses/pcdfeaa/resources/C5_PCD_FEEA_ClusterGridComputing_en.pdf

### **Shared Computers**

These are servers (groups of computers) that are shared with other people that you can connect to from your computer (typically using the internet) to help you perform more intensive computational tasks or to store large amounts of data. 

 Among shared computers there are three major options: 

1) Clusters - institutional or national resources
2) Grids - institutional or national resources
3) "Cloud" - commercial or national resources

AVOCADO - maybe put the image here for shared computers - check how anvil images were added within lists

1) [Computer Cluster](https://en.wikipedia.org/wiki/Computer_cluster)

In a computing cluster several of the **same** type of computer (often in close proximity and connected by a local area network rather than the internet) work together to perform pieces of the same single task simultaneously. The idea of performing multiple computations simultaneously is called [parallel computing](https://en.wikipedia.org/wiki/Parallel_computing).

There are different designs or architectures for clusters. One common one is the [Beowulf cluster](https://en.wikipedia.org/wiki/Beowulf_cluster) in which a master computer (called front node or server node) breaks a task up into small pieces that the other computers (called client nodes or simply nodes) perform. 

For example, if a large file needs to be converted to a different format, pieces of the file will be converted simultaneously by the different nodes. Thus each node is performing the **same task** just with different pieces of the file. The user has to write code in a special way to specify that they want parallel processing to be used and how. 

It is important to realize that the CPUs in each of the node computers connected within a cluster are all performing a similar task simultaneously.

See [here](https://cs.wmich.edu/~elise/courses/cs626/s09/hussein/Parallel_and_Cluster_Computing.pdf) for more information.

2) [Computer Grid](https://hazelcast.com/glossary/grid-computing/)

In a computing grid **different** types of computers (often in different locations) work towards an overall common goal by performing **different** tasks. 

The concept for grid computing is similar to that of an [electric power grid](https://en.wikipedia.org/wiki/Electrical_grid), where only computers (nodes) actively performing a task are using resources at any given time. 

Again, just like computer clusters, there are many types of architectures that can be rather simple to very complex. For example you can think of different universities collaborating to perform different computations for the same project. One university might perform computations using gene expression data about a particular population, while another performs computations using data from another population. Importantly each of these universities might use clusters to perform their specific task.

Both grids and clusters use a special type of software called middleware to coordinate the various computers involved.
Users need to write their scripts in a way that can be performed by multiple computers simultaneously. Users also need to be conscious of how to schedule their tasks and to follow the rules and etiquette of the specific cluster or grid that they are sharing. 

See [here](https://pediaa.com/difference-between-cluster-and-grid-computing/) for more information about the difference between clusters and grids.
 
 
AVOCADO maybe add as a reference https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=1300502


3) ["Cloud" computing](https://en.wikipedia.org/wiki/Cloud_computing)] https://go.cloudhealthtech.com/eb-simplify-the-journey-data-center-to-public-cloud.html
https://www.geeksforgeeks.org/difference-between-grid-computing-and-cluster-computing/

More recently, commercial ["Cloud"](https://en.wikipedia.org/wiki/Cloud_computing) solutions are becoming a more viable hardware solution, offered by companies like Amazon, Google, and Microsoft. This option is technically also a shared computer situation. Somewhere these companies have clusters of computers that paying customers use through the internet. In addition there are options like Jetstream which is a more "Cloud-like" part of Xsede.

AVOCADO need a new shared computer image

### Accessing Shared Computer Resources

All of the shared computing options that already exist and that you could utilize involve a [data center](https://en.wikipedia.org/wiki/Data_center) where are large number of computers are physically housed. 

![](images/taylor-vick.jpg)

Photo by [Taylor Vick](https://unsplash.com/@tvick?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/data-center?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText)

You may have access to a [HPC (which stands for High Performance Computing) cluster](https://www.hpc.iastate.edu/guides/introduction-to-hpc-clusters/what-is-an-hpc-cluster) at your institute. Or you could consider using national resources like [Xsede](https://www.xsede.org/).

Your university or institution may have a HPC [cluster](https://en.wikipedia.org/wiki/Computer_cluster), this means that they have a group of computers acting like servers that people can use to store data or assist with intensive computations. Often institutions can support the cost of many computers within an HPC cluster, allowing for what is called parallel computing. This means that multiple computers will simultaneously perform different parts of the computing required for a given task, thus significantly speeding up the process compared to you trying to perform the task on just your computer! This is also a much more cost effective option than having one expensive supercomputer (a computer that individually has the computational power of many personal computers) to act as a server. It turns out that buying several less powerful computers is cheaper.

AVOCADO - update image below to say cluster and grid access

![](images/Shared.png) 

Alternatively, you could consider an option like [Xsede](https://www.xsede.org/).
[Xsede](https://www.xsede.org/) is led by the University of Illinois National Center for Supercomputing Applications (NCSA) and includes 18 other partnering institutions (which are mostly other universities). Through this partnership, they currently support 16 supercomputers. Universities and non-profit researchers in the United States can request access to their computational and data storage resources.


Here you can see a photo of Stampede2, one of the supercomputers that members of Xsede can utilize.

![](images/Stampede2.jpg)

[[source](https://www.xsede.org/ecosystem/resources)]

> Stampede2, generously funded by the National Science Foundation (NSF) through award ACI-1134872, is one of the Texas Advanced Computing Center (TACC), University of Texas at Austin's flagship supercomputers.

See [here](https://portal.xsede.org/tacc-stampede2) for more information about how you could possibly connect to and utilize Stampede2.


Importantly when you use shared computers like national resources like Stampede2 available through Xsede, as well as institutional HPC clusters, you will share these resources with many other people and so you need to learn the proper etiquette for using and sharing these resources. These will vary by the shared resource, however in general:

1) Don't use all nodes if you don't need to
2) Don't use all RAM on a node if you don't need to
3) Communicate with others if you will be submitting a large or intensive job


### **Cloud Computing** 


https://go.cloudhealthtech.com/eb-simplify-the-journey-data-center-to-public-cloud.html
https://www.geeksforgeeks.org/difference-between-grid-computing-and-cluster-computing/


More recently, commercial ["Cloud"](https://en.wikipedia.org/wiki/Cloud_computing) solutions are becoming a more viable hardware solution, offered by companies like Amazon, Google, and Microsoft. This option is technically also a shared computer situation. Somewhere these companies have clusters of computers that paying customers use through the internet. In addition there are options like Jetstream which is a more "Cloud-like" part of Xsede.


What is the difference between the "Cloud" and other shared computer options?




![](images/Cloud.png)

## Choosing a Computing Platform

Choosing a [computing platform](https://en.wikipedia.org/wiki/Computing_platform) depends on many different considerations.  

![](images/Considerations.png)

### Important questions 

Asking yourself and your research team these questions can help you find the right computing platform:

1) Do I need a [graphical interface](https://www.omnisci.com/technical-glossary/graphical-user-interface), a [command line interface](https://searchwindowsserver.techtarget.com/definition/command-line-interface-CLI), or both?

What do we mean by this?

A [graphical interface](https://www.omnisci.com/technical-glossary/graphical-user-interface) or graphical user interface or GUI, allows for users to choose functions to perform by interacting with visual representations. They have a "user-centered" design that creates a visual environment where users can for example click on tabs, boxes, or icons for to perform functions.

[Galaxy](https://usegalaxy.org/) offers a graphical interface for performing analyses and tasks. For example in the following image we show a GUI for joining two files:

![](images/Galaxy.png)


A [command line interface](https://searchwindowsserver.techtarget.com/definition/command-line-interface-CLI) (also known as a character interface) allows for software functions to be performed by specifying through commands written in text. This typically offers more control than a graphical interface, however command line interfaces are often less user friendly as they require that the user know the correct commands to use.

For example, one could perform functions in R using Bioconductor packages such as [Biostrings](https://bioconductor.org/packages/release/bioc/html/Biostrings.html) with a command line interface:

![](images/Biostrings.png)


A situation where you might use **both** a command line interface and a GUI, is using [RStudio](https://en.wikipedia.org/wiki/RStudio) to perform an analysis in R with Bioconductor packages. [RStudio](https://en.wikipedia.org/wiki/RStudio) is what is called an IDE or an [integrated development environment](https://en.wikipedia.org/wiki/Integrated_development_environment), which is an application that supports writing code. There are many tools to help you including a console for writing code in R with command line interfacing, as well as graphical interface tools. As shown in this example below, one can inspect and save a plot (that was created with the command line) by using a GUI.

![](images/both.png)
2) Am I working with protected data that requires special security precautions?

If you are working with data that might be protected by [HIPAA](https://www.hipaajournal.com/hipaa-compliance-checklist/), such as electronic health records, then special security measures are required to ensure that only authorized users have access to the data.

![](images/HIPAA.jpg)
[[source](https://www.paubox.com/blog/what-is-hipaa/)]

3) How computationally intensive are my tasks? 

If you have a large amount of data and/or are performing complex analyses, you may require more computational power than your current laptop can provide. If this is the case, you might consider using a local server or what is called "Cloud" computing (more on that later). 


![](images/computationally_intensive.png)

4) How much storage space do I need for both temporary and long-term data?

![](images/Storage.png)

If you are working with large datasets you may also need storage options that go beyond what you currently have available. Local or "Cloud" storage options may work for you, depending on other considerations (security, data transfers) that we will discuss further.


Avocado - I want to modify this to highlight the difference between cloud computing by companies vs Xsede

1) Are my local resources sufficient? 

When a local solution already works, one may rightly question the time required to migrate to the Cloud.  However, when local solutions are insufficient or unsustainable, then the Cloud becomes a competitive option.

2) Am I working with especially big or controlled access datasets? 

Increasingly large datasets like the NCBI Sequence Read Archive are being stored on the Cloud.  If your work relies on being able to access the entire dataset, then the Cloud may be your only practical option.  Furthermore, if you work with controlled access data, then more platforms are providing compliance with regulations like HIPAA and FedRAMP.

3) Do I need to work with collaborators?  Computational research increasingly involves larger and larger collaborations.  While many fragmented systems exist to share work, the Cloud presents an opportunity for everyone to share the exact same computational environment including hardware, software, and datasets.

If Cloud Computing makes sense for you, then you’re in luck!  The past decade has seen the development of many efforts to make Cloud computing, easier, faster, and more affordable.  As each platform has their strengths and weaknesses, we will now discuss several opportunities and challenges that Cloud computing presents in the field of computational genomics.

### Benefits of Cloud Computing

The state of Cloud computing is continually evolving.  Here, we highlight three main current benefits:

https://jetstream-cloud.org/files/Jetstream-Outreach-C2Exchange-Sep2019.pdf

1) **Sharing Workflows**  

The first major benefit is the increasing ease with which one can share and collaborate on research projects. Shown here is the History feature of [Galaxy](https://usegalaxy.org/). Using this, one can share not only what datasets they used but also every computational manipulation that was performed.

![](images/Galaxy_history.png)

By sharing such a history, one can reproduce an analysis in its entirety, allowing collaborators to offer comments and extend upon the work with ease.

 

2) **Sharing Workflows between Platforms**

While sharing complete analysis histories is for the most part constrained to a particular software platform, a second benefit that has arisen is the ability to share Workflows between platforms.

Shown here is a diagram of a single cell analysis pipeline published by the Klarman Cell Observatory on Dockstore:

![](images/workflow.png)

This higher level abstraction coupled with container technology allows this multistep analysis to be run with relative ease on supporting platforms like Terra or DNAnexus.


3) **Using Commodity Hardware**

The third Benefit we highlight is the increasing ease by which one can provision commodity hardware at scale.  

![](images/cloud_Services.png)


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


## Local Costs

## Cloud Costs



