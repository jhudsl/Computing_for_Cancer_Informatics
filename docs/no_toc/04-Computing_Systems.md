



# Computing Resources

In this chapter we will describe the basics about data size and computing capacity. We will discuss the computing and storage requirements for many types of cancer-related data, as well as options to perform informatics work that might require more intensive computing capacity than your personal computer.


<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf96b1d997a_0_9.png" alt="Learning Objectives: 1. Name units of size for binary data, 2. State the computing and storage capacity of typical computers today, 3. Determine the range of storage and computing capacity required for various bioinformatics studies, 4. Recognize different methods for performing intensive computations or storing large data, 5. Explain how server and cloud computing works" width="100%" style="display: block; margin: auto;" />


## Data Sizes

Recall that the smallest unit of data is a bit, which is either a zero (0) or a one (1). A group of 8 bits is called a byte, and most computers, phones, and software programs are constructed or designed in a way to accommodate groups of bytes at a time. For example a 32-bit machine can work with 4 bytes at a time and a 64-bit can work with 8 bytes at a time. But how big is a file that is 2 GB? When we sequence a genome, how large is that in terms of binary data? Can our local computer work with the size of data that we would like to work with?



First, let's take a look at how the size of binary data is typically described and what this means in terms of bits and bytes:



<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_8.png" alt="Table of different binary data units showing the name, abbreviation, and size in bits or bytes, for example a Byte is abbreviated as B and this represents 8 bits, while Gigabyte is abbreviated GB and represents roughly 1 billion bytes" width="100%" style="display: block; margin: auto;" />


<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb6624a387_0_1.png" alt="Cartoon - One character says:Hey I'm so stoked. I have a super cool computer now, it has yodabytes. The other character says: Do you mean yottabytes. The original character says: Nope, I have lots of files about Yoda! The other character says: Oh dear..." width="100%" style="display: block; margin: auto;" />

Now that we know how to describe binary data sizes, let's next think about how much computing capacity typical computers have today.

## Computing Capacity

We have discussed a bit about CPUs and how they can help us perform more than one task at a time, but how many simultaneous tasks can the CPU of an average computer perform these days? How much memory and storage do they typically have? What size of files can a typical computer handle? These information regarding the computer's capacity and efficiency are sometimes called the **specs** of a computer.

"Typical" or "average" specs of a computer will probably change very soon, and different computers vary widely, but currently:

- **Laptops** can often perform 4-8 CPU tasks at once, and typically range from 4-16 GB in memory and 250 GB-1 TB of storage. 

This means that typical laptops can multitask quite well, have in some cases 16 gigabytes for random access memory to allow the CPU to work on relatively large tasks (as we can see from the previous table that GB are actually pretty large when you think about it), and possibly 1TB for the hard drive (and/or SSD), meaning that you can store thousands of photos and files like PDFs, word documents, etc. It turns out that 250GB allows you to store around 30,000 average-size photos, so a 1TB laptop can store quite a large amount of data. Therefore, overall, typical laptops today are pretty powerful devices, especially compared to computers of previous generations. That being said, note that some programs require 16 or even 32 GB of memory to run.


- **Desktops** can perform and store data similarly to laptops. However, they sometimes have slightly better performance and storage compared to a laptop for a similar price.  Since less work needs to be done to make the desktop small and portable, sometimes you can get better storage and performance for the same price as a laptop. Furthermore, desktops often have better graphics processing capacity and displays [@antonio_villas-boas_laptops_2019].  This might be important to consider if you are going to need to visually inspect many images. Another benefit is that you can also sometimes find desktops with larger memory and storage options right off the shelf than typical laptops. It is also generally easier to add more memory to a desktop than it is to add to a laptop [@antonio_villas-boas_laptops_2019]. However of course, desktops certainly aren't super portable!



* Some **phones** can compete with laptops by performing 6 CPU tasks at once and storing 6 GB in memory and 250 GB of storage.  


<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g1084414e81e_0_0.png" alt="Cartoon - One character says: Hey, are you moving?. The other character says: Na, I’m just bringing my computer to work, I do it everyday. It shows the character with a wheel barrel with a desktop computer in it." width="100%" style="display: block; margin: auto;" />



Check out this [link](https://www.apple.com/mac/compare/?modelList=iMac,MacBook-Pro-14,MacBook-Pro-16-2021) to compare the prices of different Macs and this [link](https://www.hp.com/us-en/shop/slp/weekly-deals) to compare specs for PC computers from HP. 


If you want to get really in-depth comparisons between different PC or Windows computers, check out this [link](https://www.userbenchmark.com/PCBuilder/Custom/S0-M1487712vsS0-M?tab=RAM) [@userbenchmark].




### Checking your computer capacity - Mac

Now, what about __your__ computer? How do you know how many cores it has or how much memory and storage it has?

If you have a Mac, you can click on the apple symbol on the far left of your screen. Then click on the "About This Mac" button.

You might see something like this:

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_69.png" alt="Result of pressing `About this Mac` button of a typical Mac today" width="100%" style="display: block; margin: auto;" />

First, we see the operating system is called MacOS Mojave.

Next, we see that the processor (which we now know is the CPU) is a 2.6 GigaHertz (GHz) Intel Core i7 chip. This means that the processor or CPU can process 2,600,000,000 operations in a second (this is called a [clock cycle](http://www.techopedia.com/definition/5498/clock-cycle)) [@clock_cycle]. That's a lot compared to older computers in the 1980s, which had clock cycle rates or [clock rates](https://en.wikipedia.org/wiki/Clock_rate) in the MegaHertz range [@clock_rate]!
If we look deeper into this chip, we would learn that it has 4 cores and has hyper-threading. This allows it to effectively perform 8 tasks at once [@hyperthreading].
Below, we see that there are 16 Gigabytes of memory - this is how much RAM it has - and also 2133 MegaHertz (aka 2.133 GHz) of low power double data rate random access memory (LPDDR3). This means that the RAM can process 2,133,000,000 commands every second [@RAM_speed; @mukherjee_ram_2019]. You can checkout more about what this means at this blog post @scott_thornton_RAM. Generally evaluating the amount of RAM is helpful in assessing performance [@RAM_speed; @mukherjee_ram_2019]. 


If we click on the storage button at the top, we can learn about how much storage is available on the computer. If you hover over a section, it tells you what type of files are accounting for that particular section of storage that is being used.

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_80.png" alt="Mac storage information showing 1 TB capactity" width="100%" style="display: block; margin: auto;" />

### Checking your computer capacity - Windows/PC


If you have a PC or Windows computer, the steps may vary depending on your operating system, but try the following:

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_96.png" alt="Windows/PC Start button" width="100%" style="display: block; margin: auto;" />

1. click the "Start" button (It's the button on the bottom left that looks like a grid with 4 squares together)
2. click "Settings" button (It's gear-shaped)
3. click "System"
4. click "About"

See this [link](https://www.businessinsider.com/how-to-find-computer-specs-windows-10) for more information.


<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_90.png" alt="Windows/PC about section" width="100%" style="display: block; margin: auto;" />

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_107.png" alt=" Example of a Windows/PC computer processor and memory information" width="100%" style="display: block; margin: auto;" />

Here we can see that this computer has an Intel(R) Core(TM) i7-4790K CPU @ 4.00 GHz 4.00 GHz chip and 16 Gigabytes of RAM.
If we look up this chip we can see that it has 4 cores and 8 threads (due to hyper-threading) allowing for 8 tasks at a time. 

To find out more information about your storage, click the "Storage" button within the "System" tab.

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_114.png" alt="Windows/PC storage information showing 1 TB capactity" width="100%" style="display: block; margin: auto;" />

Here we can see that this computer has 466 GB + 465 GB = 932 GB across the two drives. The **C: drive** is typically for the operating system, and the **D: drive** is typically where you would install application programs and save files. There are 1000 GB in a TB; therefore, we can see that this computer has about the same storage as the Mac that we just looked at.

## File Sizes

Now let's think about the files that we might need for our research, how big are files typically for genomic, imaging, and clinical research?

Recall this table from earlier about digital data size units:

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_8.png" alt="Table of different binary data units showing the name, abbreviation, and size in bits or bytes, for example a Byte is abbreviated as B and this represents 8 bits, while Gigabyte is abbreviated GB and represents roughly 1 billion bytes" width="100%" style="display: block; margin: auto;" />

### Genomic data file sizes

Genomic data files can be quite large and can require quite a bit of storage and processing power.

Below is a table of the approximate sizes of some common file types:

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_0.png" alt="Table of file types for genomics data, whole genome sequencing can become larger than the capacity of your computer with less than 20 samples! Even whole exome sequenceing can already require more than 44% of a 1TB hard drive for just 20 samples. Note that these are approximate values." width="100%" style="display: block; margin: auto;" />



### Imaging Data File Sizes

Imaging data, although often smaller than genomic data, can start to add up quickly with multiple images and samples.

Here is a table of average file sizes for various medical imaging modalities from @liu_imaging_2017:

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_35.png" alt="Table of file types for imaging data, most modalities have files in the range of MB to GB. Note that these are approximate values." width="100%" style="display: block; margin: auto;" />
[[source](https://www.mdpi.com/2078-2489/8/4/131)]


Note that depending on the study requirements, several images may be needed for each sample. Therefore, data storage needs can add up quickly.


<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_25.png" alt="Example table of overall file storage needs for samples in imaging studies." width="100%" style="display: block; margin: auto;" />


### Clinical Data File Sizes

Really large clinical datasets can also produce sizable file sizes. For example the [Healthcare Cost and Utilization Project (HCUP) National (Nationwide) Inpatient Sample (NIS)](https://www.hcup-us.ahrq.gov/db/nation/nis/nisdbdocumentation.jsp) contains data on more than seven million hospital stays in the United States with regional information.

According to the NIS website, it "enables analyses of rare conditions, uncommon treatments, and special populations" [@NIS].

Looking at the [file sizes](https://www.hcup-us.ahrq.gov/db/state/sedddist/sedddist_filesize.jsp) for the NIS data for different states across years, you can see that there are files for some states which can be as large as 24,000 MB or 2.4 GB for California [@NIS]. You can see how this could add up across years and states quite quickly.


<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gfb2e21ecdc_0_42.png" alt="Table of file sizes for the Healthcare Cost and Utilization Project (HCUP) National (Nationwide) Inpatient Sample (NIS) of data from different years and states." width="100%" style="display: block; margin: auto;" />

### Checking file sizes on Mac


If you own a Mac and want to check the size of a particular file, you can find it by locating your file within a finder window. You can open a new finder window by clicking on the button that looks like a square with two colors and a face (see image below), typically in the bottom left corner on your dock (the strip of icons on your Mac screen) to help you navigate to different application programs.


<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_120.png" alt="Mac finder button" width="100%" style="display: block; margin: auto;" />
Once you open a finder window, you can navigate to one of your files. 

If you have the view setting that looks like 4 lines, you will get information about the size of each file. 
<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_133.png" alt="Finder windows show file sizes on a Mac" width="100%" style="display: block; margin: auto;" />



You can right click on  a file and click the "Get Info" button. This will give you more specific information.

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_128.png" alt="Right clicking on a file in the finder window can give you more info about a file." width="100%" style="display: block; margin: auto;" />


### Checking file sizes on PC/Windows

Similar to the process of checking file sizes on a Mac, if you're using a Windows or PC computer, you can navigate to your files by first opening the File Explorer application by typing this in the search bar next to the "start" button.

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_139.png" alt="Finding the File Explorer on a Windows/PC computer" width="100%" style="display: block; margin: auto;" />


Then navigate to your file of interest, which will show information about the size in one of the columns to the right. If you hover over the file name, you will get more specific information.

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_145.png" alt="File sizes are listed for each file within File Explorer windows on Windows/PC computers" width="100%" style="display: block; margin: auto;" />


## Computing Options

### **Personal computers**

These are computers that your lab might own, such as laptops or desktops, used by one individual or maybe a few individuals in your lab.  

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_3.png" alt="A computer chip is also called the CPU. Inside this CPU or chip  are often multiple cores, which are actually individual CPUs." width="100%" style="display: block; margin: auto;" />


If you are not performing intensive computational tasks, it is possible that you will only need personal computers for your lab. However, as your project expands and you start working with more and complex data, you might require connecting your personal computers to shared computers for more computational power and/or storage.


### **Shared Computing Resources**

What if you decide that you need more computational power than your personal computer? You may encounter times where certain informatics tasks take way too long or are not even possible. Evaluating the potential file sizes of the data that you might be working with is a good place to start. However, keep in mind that sometimes certain computations may require more memory than you expect. This is particularly true when working with genomic or image files which are often compressed. What can you do when you face this issue?

One great and affordable option is to use a server.

Hardware-wise, the term [server](https://techterms.com/definition/server) means a computer (often a computer that has much more storage and computing capacity than a typical computer) or groups of computers that can be accessed by other computers using a local network or the internet to perform computations or store data [@server_def]. They are often shared by people, and allow users to perform more intensive computational tasks or store large amounts of data. Read [here](https://en.wikipedia.org/wiki/Server_(computing)) to learn more [@server_2021]. 

Using a group of computers is often a much more cost-effective option than having one expensive supercomputer (a computer that individually has the computational power of many personal computers) to act as a server [@supercomputer_2022]. It turns out that buying several less powerful computers is cheaper. In some cases however, an institute or company might even have a sever with multiple supercomputers!


For example, your lab members could connect to a server from their own computers to allow each of them more computational power. Typically computers that act as servers are set up a bit differently than our personal computers, as they do not need the same functionality. These computers are designed to optimize data storage and computational power. For instance, they often don't have capabilities to support a [graphical user interface](https://www.omnisci.com/technical-glossary/graphical-user-interface), meaning the visual display output that you see on your personal computer [@GUI]. 


Instead, they are typically only accessed by using a [command-line interface](https://en.wikipedia.org/wiki/Command-line_interface), meaning that users write code instead of using buttons like they might for a program like Microsoft Word that uses a graphical user interface [@command-line_2022]. In order to support this they have memory, processors or CPUs, and storage, like your laptop.

Here is what a server might look like:

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_58.png" alt="A physical server is a group of computers somewhere that connects to other computers. Such a server looks something like this." width="100%" style="display: block; margin: auto;" />

In this case we have a group of computers making up this server. Here we see the nodes (the individual computers that make up the server) stacked in columns. 


Among shared computing resources/servers, there are three major options: 

* **Clusters** - institutional or national resources
* **Grids** - institutional or national resources
* **Cloud** - commercial or national resources


### Computer Cluster

In a [computing cluster](https://en.wikipedia.org/wiki/Computer_cluster), several of the **same** type of computer (often in close proximity and connected by a local area network with actual cables or an [intranet](https://www.igloosoftware.com/blog/internet-vs-intranet-vs-extranet-whats-the-difference/) rather than the internet) work together to perform pieces of the same single task simultaneously [@computer_cluster_2022]. The idea of performing multiple computations simultaneously is called [parallel computing](https://en.wikipedia.org/wiki/Parallel_computing) [@parallel_2021].

There are different designs or architectures for clusters. One common design is the [Beowulf cluster](https://en.wikipedia.org/wiki/Beowulf_cluster) in which a master computer (called front node or server node) breaks a task up into small pieces that the other computers (called **client nodes** or simply **nodes**) perform [@beowulf_2022]. 

For example, if a large file needs to be converted to a different format, **pieces** of the file will be converted simultaneously by the different nodes. Thus, each node is performing the **same task** just with different __pieces__ of the file. The user has to write code in a special way to specify that they want parallel processing to be used and how they want this parallel processing to be performed. See [here](https://www.freecodecamp.org/news/how-to-supercharge-your-bash-workflows-with-gnu-parallel-53aab0aea141/) for an introduction about how this is done @Zach_Caceres_GNU_Parallel_2019.

It is important to realize that the CPUs in each of the node computers connected within a cluster are all performing a similar task simultaneously.

See [here](https://cs.wmich.edu/~elise/courses/cs626/s09/hussein/Parallel_and_Cluster_Computing.pdf) for more information [@de_doncker].

### Computer Grid

In a [computing grid](https://hazelcast.com/glossary/grid-computing/) are often **different** types of computers in **different** locations work towards an overall common goal by performing **different** tasks [@grid]. 

Again, just like computer clusters, there are many types of architectures that can be rather simple to very complex. For example you can think of different universities collaborating to perform different computations for the same project. One university might perform computations using gene expression data about a particular population, while another performs computations using data from another population. Within one location, each of these universities might use clusters to perform their specific task.

Both grids and clusters use a special type of software called **middleware** to coordinate the various computers involved.
Users need to write their scripts in a way that can be performed by multiple computers simultaneously. Users also need to be conscious of how to schedule their tasks and to follow the rules and etiquette of the specific cluster or grid that they are sharing (more on that soon!). 

See [here](https://pediaa.com/difference-between-cluster-and-grid-computing/)  and [here](https://www.geeksforgeeks.org/difference-between-grid-computing-and-cluster-computing/)for more information about the difference between clusters and grids [@lithmee_difference_2018;  @grid_cluster_difference_2019].
 
 
### "Cloud" computing

More recently, the ["Cloud"](https://en.wikipedia.org/wiki/Cloud_computing) has become a common computing option. The term "cloud" has become a widely used buzzword [@cha_cloud_2015] that actually has a few slightly different definitions that have changed overtime, making it a bit tricky to keep track of. However,  "cloud" typically describes large computing resources that involve the connection between **multiple servers** in multiple locations [@cloud_2022] using the internet. See [here](https://www.redhat.com/en/topics/cloud-computing/cloud-vs-virtualization) for a deeper description of what the term cloud means today and how cloud computing compares to other more traditional shared computing options [@cloud_deeper].


Many of us use cloud storage regularly for Google Docs and backing up photos using iPhoto and Google. Cloud computing for research works in a similar way to these systems, in that you can perform computations or store data using an available server that is part of a larger network of servers. This allows for even more computational dependability beyond a simpler cluster or grid. Even if one or multiple servers are down, you can often still use the other servers for the computations that you might need. 

Furthermore, this also allows for more opportunity to scale your work to a larger extent, as there is generally more computing capacity possible with most cloud resources [@cloudvstrad].



Companies like Amazon, Google, Microsoft Azure, and others provide cloud computing resources. **Somewhere these companies have clusters of computers that paying customers use through the internet.**  In addition to these commercial options, there are occasionally national government funded resource options (described in the next section).  We will compare computing options in another chapter coming up.





<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_28.png" alt="Cloud computing options" width="100%" style="display: block; margin: auto;" />


### Accessing Shared Computer Resources

It's important to remember that all of the shared computing options that we previously described involve a [data center](https://en.wikipedia.org/wiki/Data_center) where a large number of computers are physically housed. 

<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_23.png" alt="Examples of servers or shared computers include clusters  that may exist at your institution or national computing resources" width="100%" style="display: block; margin: auto;" />


You may have access to a [HPC (which stands for High Performance Computing) cluster](https://www.hpc.iastate.edu/guides/introduction-to-hpc-clusters/what-is-an-hpc-cluster) at your institute. This can be a great cost-effective and typically secure option.  


If your university or institution has a HPC [cluster](https://en.wikipedia.org/wiki/Computer_cluster), this means that they have a group of computers acting like a server that people can use to store data or assist with intensive computations. Often institutions can support the cost of many computers within an HPC cluster. This means that multiple computers will simultaneously perform different parts of the computing required for a given task, thus significantly speeding up the process compared to you trying to perform the task on just your computer! 



If your institute doesn't have a shared computing resource like the HPCs we just described, you could also consider a national resource option like the [Texas Advanced Computing Center (TACC)](https://en.wikipedia.org/wiki/Texas_Advanced_Computing_Center) which was funded by the National Science Foundation (NSF) [XSEDE](https://www.xsede.org/) program.
Universities and non-profit researchers in the United States can request access to their computational and data storage resources. Other resource options include:


- [San Diego Supercomputer Center (SDSC)](https://www.sdsc.edu/) at the University of California, San Diego
- [National Institute for Computational Sciences (NICS)](https://www.nics.tennessee.edu/), at the University of Tennessee, Knoxville
- [Pittsburgh Supercomputing Center (PSC)](https://www.psc.edu/) at the Carnegie Mellon University and University of Pittsburgh


Here you can see a photo of Stampede2, one of the supercomputers that members of TACC could utilize (it has now been replaced with Stampede3).


<img src="04-Computing_Systems_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf9c252d058_0_63.png" alt="An image of Stampede2 one of the supercomputers that members of TACC could use." width="100%" style="display: block; margin: auto;" />


[[source](https://www.xsede.org/)]

> Stampede2, generously funded by the National Science Foundation (NSF) through award ACI-1134872, is one of the Texas Advanced Computing Center (TACC), University of Texas at Austin's flagship supercomputers.



See [this article about Stampede2 and the transition to Stampede3](https://tacc.utexas.edu/news/latest-news/2023/07/24/taccs-new-stampede3-advances-nsf-supercomputing-ecosystem/) for more information about their resources and see [their getting started website](https://tacc.utexas.edu/use-tacc/getting-started) on how you could possibly use their resources.

Importantly when you use shared computers like national resources like [Stampede2](https://tacc.utexas.edu/systems/stampede2/) and [Stampede3](https://docs.tacc.utexas.edu/hpc/stampede3/), as well as institutional HPCs, you will share these resources with many other people and so you need to learn the proper etiquette for using and sharing these resources. We will discuss this more in a coming chapter.

There is also an option to access national computing resources through a cloud environment option called [Jetstream2](https://jetstream-cloud.org/).  



Here is a video about Jetstream2:

<iframe src="https://www.youtube.com/embed/NQ3flxJANTw" width="100%" height="400px" data-external="1"></iframe>




We will also discuss how the use of these various computing options differ in the next chapters. Importantly there are also some computing platforms that have been specially designed for scientists and specific types of researchers, so it is also useful to know about these options.



## Conclusion

We hope that this chapter has given you some more perspective on how large medical research data files can be, and has made you more familiar with how well your computer can accommodate the files that you might work with. We also hope that this chapter has provided you with more awareness about computing options that might be available to you, should you need more capacity than your current computer. 

In conclusion, here are some of the major take-home messages:

1) A bit is the smallest binary digital data unit. It is a single 0 or 1.
2) A byte is composed of 8 bits. File sizes are typically described using units based on bytes.
3) A typical fancy laptop today might allow for up to 1 TB of storage; however, this can quickly get used up if you are working with large data files. 
4) Even if you have enough storage for a large file, you might not have enough RAM to work with a large data file. Your computer might be too slow to handle that type of work. In this case, you might want to consider using shared computing resources.
5) A server, when describing hardware, is a single computer (typically a supercomputer) or group of computers that others can share to help them perform more intensive computational tasks or store large amounts of data. People often connect to servers over the internet, but one can also directly connect to servers in a local network (for example, in different offices in a department or a company).
6) Computers in a server are optimized for assisting users with computations or storing data.
7) A supercomputer is a computer that has much more storage, memory, and computing capacity than a typical personal computer. Supercomputers are generally much more expensive than using a group of more typical computers that together would have the same collective computing and storage capacity.
8) There are two general types of servers: clusters and grids. Cluster approaches work by having several computers working on pieces of the same task simultaneously in a method called parallel computing. Grid approaches work by having different types of computers working on different tasks. 
9) Cloud computing is essentially the use of many servers accessed through the internet. This is often more reliable because there are many servers to use, even if one other users are performing large tasks or if a server goes down. We will talk more about the pros and cons of this option in the coming chapters.
10) If your institute doesn't provide you access to a shared computing resource and you don't want to use a commercial cloud option, you could consider options like [TACC](https://en.wikipedia.org/wiki/Texas_Advanced_Computing_Center) and or [Jetstream2](https://jetstream-cloud.org/), which is a national resource that you can request access to.



