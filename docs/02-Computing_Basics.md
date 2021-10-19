---
title: "02-Computing_basics"
output: html_document
---

# Computing basics

In this chapter we will describe the basics about computing, what cloud computing actually is, and methods to perform informatics work that might require more intensive computing.

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_4.png" title="Learning Objectives: 1. Describe the basics of how computers work, 2. Define basic computing terminology, 3. Recognize different methods for performing intensive computations, 4. Explain the difference between cloud computing and local computing" alt="Learning Objectives: 1. Describe the basics of how computers work, 2. Define basic computing terminology, 3. Recognize different methods for performing intensive computations, 4. Explain the difference between cloud computing and local computing" width="100%" />

First we would like to start off with some background information about how computers actually work. Understanding how computers actually work will be very helpful for understanding what computing resources your research will actually require. 


<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf5f8818810_1_166.png" title="comic: Ever wonder how computers work?It’s millions of tiny bees doing a lot of math, so you don’t have to!" alt="comic: Ever wonder how computers work?It’s millions of tiny bees doing a lot of math, so you don’t have to!" width="100%" style="display: block; margin: auto;" />


## Computing Components

Luckily, you are likely not going to need to become a bee keeper to perform your computational research (unless of course that interests you)! Instead, computers rely on millions to billions of [transistors](https://technologystudent.com/elec1/transis1.htm).




### Transistors

[Transistors](https://www.physlink.com/education/askexperts/ae430.cfm) are one of if not the most important basic building blocks of computers. There are many different types of transistors, but they often look like a rectangle with three prongs.  

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_274.png" title="Anatomy of a transistor, rectangle with with three prongs for receiving or emitting current" alt="Anatomy of a transistor, rectangle with with three prongs for receiving or emitting current" width="100%" style="display: block; margin: auto;" />


[Transistors](https://technologystudent.com/elec1/transis1.htm) behave like electronic switches or gates that either allow or do not allow current to flow through a particular part of a circuit. 


<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_10.png" title="Comic: Galdolf lego character from the Lord of the Rings saying: You shall not pass! (He is holding a large transistor.)" alt="Comic: Galdolf lego character from the Lord of the Rings saying: You shall not pass! (He is holding a large transistor.)" width="100%" style="display: block; margin: auto;" />

[[Source](https://unsplash.com/photos/9paY25EHOBo)]

Inside the plastic, is often [silicon](https://en.wikipedia.org/wiki/Silicon), or some other semiconductive crystal.  Semiconductors are needed because they can conduct electricity (especially when combined with a layer of conductive metal) but are neutral on their own, making them the perfect option for creating an electrical switch. Silicon is especially useful, because it doesn't cause the circuit to get very hot, unlike previously used materials. It is also very abundant, in fact, it is the second most common element of the Earth's crust! [@Wikipedia_Silicon]).


<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_315.png" title="Anatomy of a transistor, the rectangular part of the transistor contains silicon and metal underneath a plastic insulating layer. It does not allow much current unless the transistor is on." alt="Anatomy of a transistor, the rectangular part of the transistor contains silicon and metal underneath a plastic insulating layer. It does not allow much current unless the transistor is on." width="100%" style="display: block; margin: auto;" />

If the transistor receives a small amount of current to one of the prongs (called the base), this turns it on, and allows the larger current for the circuit to pass through the transistor (from a prong called the collector to the prong called the emitter). 

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_296.png" title="The transistor can turn on our of depending on if a small current is applied to the prong called the base. Another prong is called the collector which receives the current from the circuit and the final prong is called the emitter. It emits the current from the circuit if the transistor is on." alt="The transistor can turn on our of depending on if a small current is applied to the prong called the base. Another prong is called the collector which receives the current from the circuit and the final prong is called the emitter. It emits the current from the circuit if the transistor is on." width="100%" style="display: block; margin: auto;" />

If the base prong of the transistor does not receive a small current than the transistor is off and the current for the circuit is not allowed to flow through the transistor.

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_328.png" title="Depiction of two transistors, one is one and one is off. The one that is one recieves current to the base prong and allows the current for this part of the circuit to pass through. The transistor that is off does not recieve current to the base prong and thus the current that comes into the transistor from the circuit does not pass through" alt="Depiction of two transistors, one is one and one is off. The one that is one recieves current to the base prong and allows the current for this part of the circuit to pass through. The transistor that is off does not recieve current to the base prong and thus the current that comes into the transistor from the circuit does not pass through" width="100%" style="display: block; margin: auto;" />

These two states for the flow of current ultimately allow for the storage and use of binary data, which we think of a zeros and ones, but it is really the absence or presence of current with a voltage beyond a threshold for this part of the circuit. 

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_147.png" title="Simplified illustration of how transistors work. If the transistor is given a digital data input of 1, it allows current to flow through, with a digital output of 1. Alternatively, if the the transistor is given a digital data input of 0, it does not allow current to flow through - with a digital output of 0." alt="Simplified illustration of how transistors work. If the transistor is given a digital data input of 1, it allows current to flow through, with a digital output of 1. Alternatively, if the the transistor is given a digital data input of 0, it does not allow current to flow through - with a digital output of 0." width="100%" style="display: block; margin: auto;" />


Thus the physical components of a computer are ultimately based on the assessment of only two states of current (0 (or FALSE) = below a threshold and 1 (or TRUE) = above a threshold), which is much easier to create than if it we needed to assess more nuanced levels of current. It turns out that this is all that is needed for computers to perform all the complex tasks that we rely on them for everyday.  


Very importantly transistors have gotten much smaller over time.

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_27.png" title="Graph showing how the size of transitors has changed from about 1 centimeters in the 1950s to 1-5 nanometers today" alt="Graph showing how the size of transitors has changed from about 1 centimeters in the 1950s to 1-5 nanometers today" width="100%" style="display: block; margin: auto;" />

The smaller size of transistors has allowed for many more transistors to be used inside computers. 


<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_18.png" title="Graph showing that the number of transitors in circuit chipshas incresed from the thousands in the 1970s to 50 billion today" alt="Graph showing that the number of transitors in circuit chipshas incresed from the thousands in the 1970s to 50 billion today" width="100%" style="display: block; margin: auto;" />

[[Source](https://commons.wikimedia.org/wiki/File:Moore%27s_Law_Transistor_Count_1971-2018.png)]

Both the smaller size of the transistors and the increased number of transistors within computers have in part allowed computers to become faster and more powerful [@Pokropivny2007].


These silicon transistors became so important for the field of electronics, that the late 20th century and early 21st century is sometimes called the "Silicon Age". This is also why many places in the world where there are many technological institutes are often called a name with silicon, such as [Silicon Valley](https://en.wikipedia.org/wiki/Silicon_Valley). Here is an interesting [article](https://futurism.com/could-mark-end-silicon-age) about what our next age might be about, and it has to do with changing the way we harness electrons (the current role of transistors) - that's how important they are!


If you would like to learn more about the history of transistors and how they work check out this [website](https://www.explainthatstuff.com/howtransistorswork.html).

### ALU - Arithmetic Logic Unit

The ALU is responsible for performing simple operations by using networks (in this case commonly called a circuit) of transistors. 

These simple operations include logical operations (such as AND, OR, or NOT etc.), and arithmetic operations (such as addition, subtraction, or multiplication etc.).  

Ultimately most of what we do everyday on our computers come down to these simple operations.

These operations are based on what is called [Boolean logic or Boolean algebra](https://en.wikipedia.org/wiki/Boolean_algebra), which was invented by George Boole in 1854 and largely comes down to thinking of possible sets of data [@explainthatstuff]. For example, if we have two transistors, they could both be on, they could both be off, or one or the other could be on. Considering these possibilities, we can make overall descriptions about the flow of current to perform logical operations.
 
Let's take a moment to understand how networks of transistors work for AND and OR operations. We call a network for a logical operation a **logic gate**.


The transistor AND gate has two transistors in series, meaning they are sequentially placed one after the other, where one receives current first before the other. A resulting high current output only occurs when both of the transistors allow for the flow of current. If either or both of the transistors is off than the current is not allowed to flow through.

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_63.png" title="Illustration of logic AND gate showing transistors in series. If either or both of the transistors is off (receiving digital input of 0 in the form of no small current to base prong), then the gate  does not allow the current to flow through this part of the circuit. If both transistors are on then the current can flow through this part of the circuit." alt="Illustration of logic AND gate showing transistors in series. If either or both of the transistors is off (receiving digital input of 0 in the form of no small current to base prong), then the gate  does not allow the current to flow through this part of the circuit. If both transistors are on then the current can flow through this part of the circuit." width="100%" style="display: block; margin: auto;" />


The transistor OR gate has two transistors in parallel, meaning they are next to one another each receiving the flow of current at the same time. A resulting high current output can occur when either of the transistors allows for the flow of current.

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_217.png" title="Illustration of logic OR gate showing transistors in parallel. If either or both of the transistors is on (receiving digital input of 1 in the form of a small current), then the gate allows the current to flow through this part of the circuit." alt="Illustration of logic OR gate showing transistors in parallel. If either or both of the transistors is on (receiving digital input of 1 in the form of a small current), then the gate allows the current to flow through this part of the circuit." width="100%" style="display: block; margin: auto;" />
 


Importantly using more complex arrangements of these logic gates can allow the computer to perform the arithmetic operations. See [here](http://homepage.divms.uiowa.edu/~jones/assem/notes/08arith.shtml) and [here](
https://en.wikipedia.org/wiki/Adder_(electronics)) for more information on how this works.


If you would like to learn more about these gates with circuit diagrams, check out this [website] (http://hyperphysics.phy-astr.gsu.edu/hbase/Electronic/trangate.html#c1) and this [website](https://www.cs.bu.edu/~best/courses/modules/Transistors2Gates/) for some visualizations. This [website](https://www.explainthatstuff.com/logicgates.html) and this [website](https://www.electronics-tutorials.ws/logic/logic_1.html) also go into great detail.

In case you are wondering about the semantics of phrases like the "flow of current", check this [discussion](https://electronics.stackexchange.com/questions/61780/isnt-current-flow-a-wrong-term).


### Binary or Boolean data

An ALU performs arithmetic operations using values are represented in binary digits called bits (0 or 1) (recall that this is based on a state of current). Data like this is also called [Boolean](https://en.wikipedia.org/wiki/Boolean_algebra), because George Boole invented a system of algebra for such data in 1854 . These values do not mean their typical meanings from what we know numerically, but instead follow arithmetic rules using 2 as the base, as opposed to 10 which we are familiar with for our decimal system. What does this mean?
With our decimal system when we reach a value of 10, we start to carry over the 1. With the binary system when we reach a value of 2, we start to carry over the 1.


<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_104.png" title="Image showing how binary addition works. 0 +0 = 0, 0+1 = 1, 0+1 = 1, and 1+1 = 10. Why would this last calculation be true? It is because we can only use 0s and 1s and once we reach the value of 2 we need to carry over the 1 to left one place." alt="Image showing how binary addition works. 0 +0 = 0, 0+1 = 1, 0+1 = 1, and 1+1 = 10. Why would this last calculation be true? It is because we can only use 0s and 1s and once we reach the value of 2 we need to carry over the 1 to left one place." width="100%" style="display: block; margin: auto;" />

Here we can see how the first 9 digits of the decimal system are represented in the binary system.

<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_265.png" title="Table showing how decimal values 0-10 are represented in the binary system." alt="Table showing how decimal values 0-10 are represented in the binary system." width="100%" style="display: block; margin: auto;" />

See [here](https://www.calculator.net/binary-calculator.html) to learn more about binary calculations.


### Flip-flops and registers

Flip-flops are used for storing one bit of digital binary data. They are made of transistors (that's right it's transistors again!) in a configuration that allows for the flip-flop to hold one of two states, thus enabling the storage of binary data.

A group of flip-flops is called a register. You may have heard about a computer having a 64- or 32- bit operating system (more on what this soon). These computers have registers with 64 bits or 32 bits respectively. Thus there are 64 flip-flops within the registers of a [64-bit](https://www.computerhope.com/jargon/num/64bit.htm) system. Each of these are capable of storing and processing binary values 64 digits in length (which works out to an unsigned integer in our decimal system of up to 2^64-1, or 18,446,744,073,709,551,615)!

You may also be wondering how letters and other symbols are stored in this binary system. 

Letters are each assigned a numeric decimal value according to an encoding system such as the [ASCII system](https://www.computerhope.com/jargon/a/ascii.htm), and these are converted into the binary form of the number. In the ASCII system, this ultimately works out to letters being stored by 8 binary bits or digits also called a byte [@computerhope]. Since this is consistent, this works well with systems that have registers that can store in sets of 8 bits. Since 64 divided by 8 is 8, this means for a 64-bit operating system, each register can store 8 letters or symbols at a time.

Below you can see the decimal value for some of the symbols and letters:


<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_187.png" title="Chart showing the ASCII decimal assigned to various characters or letters and the binary number for that ASCII value. For example an upper case letter A is coded  064 in ASCII and the binary number eight bit number is 01000001." alt="Chart showing the ASCII decimal assigned to various characters or letters and the binary number for that ASCII value. For example an upper case letter A is coded  064 in ASCII and the binary number eight bit number is 01000001." width="100%" style="display: block; margin: auto;" />

Note that ASCII has largely been replaced in 1991 for [Unicode](https://en.wikipedia.org/wiki/Unicode), which allows for more characters, supporting languages like Chinese that require for more characters than the 256 that ASCII could support, however this works in a similar way.

### **CPU** - Central Processing Unit  or Core


The CPU is often called **the brain** of the computer. This is what people are referring to when they describe a "computer chip". It performs and orchestrates computational tasks. 

The CPU is made up of several components, a few that are particularly important (two of which we have discussed): 
 1) ALU  
 2) Registers  
 3) Control Unit (CU)  
 
The Control Unit coordinates the ALU and the data stored in the registers, so that the ALU can perform the operations on the right data stored in the registers at the right time.
 
Modern computers now have multiple cores. What does this mean?

This means that there are multiple CPUs within the same computer chip.  A dual core CPU is a chip with two CPUs. A quad-core CPU is a chip with 4 CPUs and so on.This allows modern computers to perform multiple tasks at the same time instead of sequentially, such as 4 tasks simultaneously on a current typical laptop (with 4 cores). This makes our computers much faster than they used to be. 

In addition to the main CPU, computers may be equipped with specialized processors called [GPUs](https://www.intel.com/content/www/us/en/products/docs/processors/what-is-a-gpu.html#) which stands for graphics processing units that are especially efficient at tasks involving images. Thus any tasks that require the involvement of images are done using the GPU and not the CPU. This frees up the CPU to continue on the tasks not involving images more efficiently.


<img src="02-Computing_Basics_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf6e632d05f_0_381.png" title="A computer chip is also called the CPU. Inside this CPU or chip  are often multiple cores, which are actually individual CPUs." alt="A computer chip is also called the CPU. Inside this CPU or chip  are often multiple cores, which are actually individual CPUs." width="100%" style="display: block; margin: auto;" />
Hyper-threading is also an option for improving processing. This technology started in 2002 by Intel. The idea is that while part of the same CPU is idle or waiting for a given task,  another part of the CPU can work to perform another task. This isn't as efficient as a having another core or CPU, but it does improve efficiency. So many modern computer chips actually use all three efficiency boosters (having multiple cores, having GPUs, and using hyper-threading). Thus a chip with 4 cores that also has hyper-threading can work on 8 tasks simultaneously. Since it is now much easier to produce chips with multiple cores and because there are some security concerns with hyper-threading, the field seems to be moving away from hyper-threading.

### **Memory or RAM** - short-term memory

OK, so we have already talked about how data can be stored in the registers within the CPU. This data or memory is used directly by the CPU during operations or tasks. However, our CPUs need additional quick access to data to tell the CPU what to do to perform the operations. This bring us to [RAM](https://www.computerhope.com/jargon/r/ram.htm).  [RAM](https://www.computerhope.com/jargon/r/ram.htm) stands for **Random Access Memory**.  It is often simply referred to as **memory**.  Since CPUs are fast, RAM needs to be fast, making it relatively expensive. One distinctive feature of this type of memory is that it is temporary. When your computer no longer has power, the data stored in RAM disappears. This type of memory is also called volatile.  

is Ram just registers located outside the CPU?

For more information about how RAM works, check out this website: https://computer.howstuffworks.com/ram.htm.

### **Storage**  - long-term memory

Avocado start motivating discussing data transfers here a bit...

We can also store data that we aren't directly using when our computer is performing operations. This type of memory is called storage and is sometimes referred to as long-term or non-volatile memory because electricity is not required to preserve this data. This type of memory is stored using [hard disk drives (HDD) also called hard drives](https://www.computerhope.com/jargon/h/harddriv.htm) or more recently [solid-state drives (SSD)](https://www.computerhope.com/jargon/s/ssd.htm). Typically ranging from gigabytes to terabytes or more, this type of storage offers big data capacity for a relatively low price at the cost of speed.

Hard disk drives store memory using magnetic methods, while solid-state drives store memory using chips that have guess what??

They are made of yet again the important basic building block of computers - tiny bees!  Oops, I mean transistors yet again, just like the CPU chip! See those transistors are really important.

SSDs allow for much faster reading and writing of files, as well as increased reliability. However, they are more expensive and they also wear out eventually. 
https://computer.howstuffworks.com/solid-state-drive.htm

Go into this??? ROM stands for **Read-Only Memory**. This means that the data remains statically stored and can only be rewritten in limited circumstances.

 https://arstechnica.com/information-technology/2012/06/inside-the-ssd-revolution-how-solid-state-disks-really-work


https://www.extremetech.com/computing/88078-how-a-hard-drive-works


### Hardware and Software
So far we have talked about the [hardware](https://simple.wikipedia.org/wiki/Computer_hardware) of a computer, while [software](https://simple.wikipedia.org/wiki/Software) is the code that tells the hardware how to function.

Software can also be important to know about. Most importantly it is useful to know about operating systems.

### Operating Systems

The [operating system](https://en.wikipedia.org/wiki/Operating_system) (sometimes simply called the OS) is a set of code or software that translates user interactions with the computer to tell the hardware (including memory and the CPU) of the computer what tasks to do and when.

You can think of this as the basic code to keep the computer running and functional and to allow the user to use other forms of software, such as applications. Applications are specialized software programs like Microsoft Word, or an internet browser like Chrome that allow a user to do specific tasks on the computer. So your OS is what allows you to name, rename, move and save files. It helps you to keep track of memory and decides what memory should be used when and to run all of your application software . It also allows you to talk to other devices like printers or other computers.

Examples of commonly used operating systems are:
* Microsoft Windows (such as Windows 10, Windows 11 etc.)
* macOS (notice the OS here - it might make more sense now why it is called this)
* Linux  
* Android

Previously, back when a university might have one single computer, as they were so large and expensive (they didn't use those nifty small transistors of today), computers didn't have operating systems and only one task could be performed at a time by one person at a time. Back then, tasks were just manually started and prioritized and scheduled by humans. Tasks or programs (including sometimes data) could be printed or punched on cards (called punched cards) that would be loaded into the machine. It could really be a pain for users if they accidentally dropped the cards for the program they wanted to run, as you can imagine!

See here for more information: https://www.deskdecode.com/operating-systems-os/

https://timeline.com/women-pioneered-computer-programming-then-men-took-their-industry-over-c2959b822523
https://spectrum.ieee.org/untold-history-of-ai-invisible-woman-programmed-americas-first-electronic-computer







Networks, cloud computing, data transfer, servers....operating systems

