---
title: "Computing Systems"
output: html_document
---




# Computing Systems

In this chapter we will describe the basics about data size, as well as methods to perform informatics work that might require more intensive computing than your personal computer.


<img src="resources/images/03-General_Platforms_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf5f8818810_1_171.png" title="Learning Objectives: 1.Describe the size of various data, 2. Recognize the difference between personal computers and remote computing options. 2.Explain how cloud computing and server computing works 3. Determine which options will provide enough computing capacity for your research needs" alt="Learning Objectives: 1.Describe the size of various data, 2. Recognize the difference between personal computers and remote computing options. 2.Explain how cloud computing and server computing works 3. Determine which options will provide enough computing capacity for your research needs" width="100%" style="display: block; margin: auto;" />

This chapter aims to provide research leaders with some guidance about general computing options, such as personal computers,  local computing clusters, and cloud options. We will discuss how networks and servers work, as well as cloud computing and we will describe the computing capacity of each option as well as other considerations. virtual machines???

## Data Sizes

Recall that the smallest unit of data is a bit which is either a zero or a one. A group of a bits is called a bite, and most computers and phones, and software programs are constructed or designed in a way to accommodate groups of bites at a time. For example a 32-bit machine can work with 4 bytes at a time and a 64-bit can work with 8 bytes at a time. But how big is a file? When we sequence a genome, how large is that in terms of binary data? Can our local computer work with the size of data that we would like to work with?


https://www.backblaze.com/blog/how-many-bytes-are-in-a-megabyte-really/
https://www.strand-ngs.com/support/ngs-data-storage-requirements
http://massgenomics.org/2014/11/brace-yourself-for-large-scale-whole-genome-sequencing.html
https://www.ridom.de/u/WGS_Data_Types_&_Sizes_and_Runtimes.html
https://www.biostars.org/p/315213/

Want examples of different relevant data sizes:
imaging data
genomic data:
- raw  fastq files
- fasta files
- bam files
- whole genome
- exome
- RNA seq
- small RNA seq
- proteomics
- methylation
- human and mouse...
clinical data


## Computer Capacity

Now that we know about the CPU, how many tasks can the CPU of an average computer do these days? How much memory and storage do they typically have?


![](images/current_comp.png)
These values will probably change very soon, but currently:

* **Laptops** can perform 8 CPU tasks at once, storing 64 GB in memory and 8 TB on storage.  
* **Handheld tablets** can now perform 8 CPU tasks, and store 6 GB in memory and 1 TB on storage. 
* Some **phones** can compete with laptops from the not so distant past by performing 6 CPU tasks at once and storing 4 GB in memory and 0.5 TB of storage.  




### Servers

What if we need to more computational power than our laptop? You may encounter times where certain informatics tasks take way too long or are not even possible on your personal computer.

In terms of hardware, the term [server](https://techterms.com/definition/server) means a computer or computers that can be accessed through a direct local network or the internet to perform computations or store data. Read [here](https://en.wikipedia.org/wiki/Server_(computing)) to learn more. 

For example, your lab members could connect to a server from their own computers to allow each of them more computational power. Typically computers that act as servers are set up a bit differently than our personal computers, as they do not need the same functionality. For instance they often don't have capabilities to support a [graphical interface](https://www.omnisci.com/technical-glossary/graphical-user-interface) (more on what that is later). They are designed to optimize data storage and computational power.

![](images/Servers.png)


## Computing Platforms

Now that we have discussed a bit about how computers perform computations, lets discuss more about how you might choose your computing platform. A computing platform, is all the [hardware](https://simple.wikipedia.org/wiki/Computer_hardware) (the physical parts of your computing platform) and [software](https://simple.wikipedia.org/wiki/Software) (the code that tells the computing platform how to function) necessary to create the environment in which you can perform your computational work.


## Hardware

With regards to hardware, there are two major options:  

1) Personal computers   
2) Shared computers   




### **Personal computers**

These are computers that your lab might own, such as a laptop, a desktop, or a small [server](https://techterms.com/definition/server) used by just your lab.  





![](images/Personal.png)


If you are not performing intensive computational tasks, it is possible that you will only need personal computers for your lab. However, you may find that this changes, and you might require connecting your personal computers to shared computers for more computational power and or storage.

Note that you could technically purchase your own server. However, this is very likely not as economical, feasible (as having your own server would require that you personally maintain it), or salable (you might outgrow your server) as other computing options that we will discuss in a bit. 


https://profs.info.uaic.ro/~adria/teach/courses/pcdfeaa/resources/C5_PCD_FEEA_ClusterGridComputing_en.pdf

### **Shared Computers or Networks**

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

More recently, commercial ["Cloud"](https://en.wikipedia.org/wiki/Cloud_computing) solutions are becoming a more viable hardware solution, offered by companies like Amazon, Google, and Microsoft. This option is technically also a shared computer situation. **Somewhere these companies have clusters of computers that paying customers use through the internet.** In addition there are options like Jetstream which is a more "Cloud-like" part of Xsede.

AVOCADO need a new shared computer image and more about Jetstream which I think is a good option for many people

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


![](images/Cloud.png)




