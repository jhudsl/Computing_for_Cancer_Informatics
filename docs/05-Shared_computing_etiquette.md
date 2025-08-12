


# Shared Computing Etiquette

In this chapter we will discuss the proper etiquette for using more traditional shared computing resources, such as an institutional high performance computing cluster server. This will help you to understand what would be required for you to use such resources. Different resources will have slightly different use rules, however, many resources will share common usage requirements. The following is written based on personal experience, the @doi_rules and the @JHPCE.


![](05-Shared_computing_etiquette_files/figure-docx//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g11383d0152c_0_12.png){width=100%}

We will use the Johns Hopkins Joint High Performance Computing Exchange (JHPCE) cluster resource as an example to motivate the need for usage rules and proper sharing etiquette for such resources.

First, let's learn a bit about this JHPCE. For this particular resource, there are about 400 active users. It is optimized for genomic and biomedical research and has 4,000 cores! That's right; as you can imagine, this is much more powerful than the individual laptops and desktops that researchers at the university have for personal use, which would currently typically only have around 8 cores. The JHPCE also has 28TB of RAM and 14 PB of storage!

Now that you know more about digital sizes, you can appreciate that this server can allow for much faster processing and really large amounts of storage, as again a researchers' computer might have something like 16 GB of RAM and 1TB of storage. 

At the time of writing, JHPCE had 68 nodes. As with most clusters, some of the nodes are dedicated to managing user access to the cluster and some of the nodes are dedicated to transferring data. Each node has 2-4 CPUs that provide 24-128 cores! As you can see, these processors or chips have a lot more cores per each CPU than a typical personal computer. 

Individual users connect and perform jobs (a.k.a. computational tasks) on the cluster using a formal [common pool resource (CPR)](https://en.wikipedia.org/wiki/Common-pool_resource) hierarchy system. What does this mean? Recall that we are talking about shared resources, where if one user overuses the resource, it would be to the detriment of other users' experiences. Rules and regulations are designed to prevent this from happening and are enforced by managers of the resource @common-pool_2022. This is important because if a single or a few users used up all the computing resources one day, then the other nearly 400 users would not be able to perform their work that day, which would not be fair. 

## General Guidelines for shared computing resources

Each cluster or other shared computing resource will have different rules and requirements, but here are a few general rules to keep in make sure that you don't accidentally abuse the privilege of sharing an amazing resource like this. Don't be too worried, as most shared resources will give you guidance about their specific rules and will often also have settings that don't allow users to make major blunders.

### Security guidelines

One major aspect to consider is keeping the computers in the cluster safe from harm. You wouldn't want to lose your precious data stored on the cluster and neither would your colleagues!

 - Use a good [secure password](https://help.lafayette.edu/guidelines-for-strong-passwords/) that is not easy for someone else to guess.
 
 Some people suggest using sentences that are easy for you to remember, you could consider a line of lyrics from song or poem that you like, or maybe a movie. Modify part of it to include symbols and numbers [@passwords].
 

![](05-Shared_computing_etiquette_files/figure-docx//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g11383d0152c_0_22.png){width=100%}

 
 - Don't share your password and keep it safe!
 
 If you have a Mac, you could consider storing it in your [Keychain](https://support.apple.com/en-ie/guide/mac-help/mchlf375f392/mac). Alternatively, if you have a different type of computer or don't like the Mac Keychain, consider options like [Dashlane](https://www.dashlane.com/) or other password manger services. Luckily the  Mac Keychain does not come at any extra cost and can be helpful for safely storing all the passwords we use regularly safely. These are especially good options if your password is too long or difficult for you to remember. Make sure that you abide by any rules regarding storing passwords that might be required by the resource you intend to use. 
 

![](05-Shared_computing_etiquette_files/figure-docx//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g10e2895be5b_58_54.png){width=100%}
 
 
 - Don't access a server on a computer that is not authorized to do so.

Some servers will require that your computer be authorized for access for added security. It's a good idea to follow these rules. If you can, perhaps authorize a laptop in case you might need to gain access when you are out of town. However, if you do so, make sure you also only access such servers with a secure WiFi network. One way to ensure this is is to avoid using public WiFi networks. If you must use a public WiFi network, consider using a [virtual private network (VPN)](https://en.wikipedia.org/wiki/Virtual_private_network) for added security. Here is an [article](https://www.wired.com/story/best-vpn/) about different VPN options [@gilbertson_4_2021].

 -  Do not alter security settings without authorization.
 
Loosening security settings could pose a risk to the data stored on the server. On the other hand, changing the security settings to become stricter could hinder other users from performing their work. Contact the managers of the resource if you think changes need to be made.

 - Immediately report any data security concerns.
 
To protect the integrity of your and your colleagues' data, be sure to report anything strange about the shared computing resource to those who manage it, so that they can address it right away. Also report to them if you experience any security breaches on the computer(s) that you use to access the shared computing resource.

### Overall use guidelines

Now that we know how to keep the resource safe, let's next talk about general usage.

 - Don't install software unless you have permission.
 
It is possible that the software you want to use might already be installed somewhere on the shared computing resource that you are unaware about. In addition, if you install a different version of a software program, it is possible that the different version (especially if it is newer) will get automatically called by other people's scripts that build on a previous version of the program. This could break their scripts or modify their results. They may have a reason to use an older version of that software, do not assume that they necessarily want the updated version. Instead, let the managers of the resource know. They can inform other users and make sure that everyone's work will not be disrupted.
 
 - Don't use the server for storage or computation that you are not authorized for.

This is often a rule for shared computing resources, simply because such shared resources are intended for a specific reason and likely funded for that reason. Such resources are costly, and therefore the computational power should be used only for its intended purpose. Using these valuable resources for other purposes can sometimes be viewed as theft.

 - Don't alter configurations without authorization.
 
This could result unintended and unexpected consequences for other users. 


### Daily use guidelines

Now let's discuss how you should use such resources on a daily basis.

When you submit jobs, make sure you follow the following guidelines. Again consider the fact that there may be more or different requirements for the specific resource that you might be using.

 - Don't use the login or transfer nodes for your computations.
 
 This will cause issues for other users in terms of logging in and transferring their data. This could cause them to be unable to do their work.
 
 - Think about memory allocation and efficiency.
 
Consider how much RAM and storage is available for people on the shared computing resource. Try not to overload the resource with a very intensive job! Jobs that use most of the resources may either slow down the efficiency of the work for others or not allow them to perform their work at all.

Specifically, the etiquette regarding memory allocation includes:

   * Not using too many nodes if you don't need to
   * Not using too much RAM on a given node or overall if you don't need to
   * Not submitting too many jobs at once
   * Communicating with others to give them advanced warning if you are going to submit large or intensive jobs
   
If you have a really large job that you need to perform, talk with the managers of the resource so that you can work out a time when perhaps fewer users would be inconvenienced. Consult the guidelines for your particular resource about how one lets people know about large jobs before you email the administrators of the resource directly. Often there are communications systems in place for users to let each other know about large jobs.

The illustration below depicts how timing can affect the user experience in using a shared resource. If many people are using the same resource at the same time, especially using up the resources with a heavy task, it might slow down other users, or hinder them from performing their jobs fully. It might be a good idea to target a time frame when you know the resource will likely be less crowded.

![](05-Shared_computing_etiquette_files/figure-docx//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g11bbe6ab7c6_0_4.png){width=100%}


### Communication Guidelines

Speaking of communication, let's dive into this subject deeper for a bit.

- Use the proper order for communication.

Often shared resources have rules about how they want people to communicate. For example, for some resources, it is suggested that you first ask your friends and colleagues if you are confused about something, then consult any available forums; if that does not work, then directly email the administrators/managers of the resource. Keep in mind that these people are very busy and get lots of emails and inquiries. 

- Use the ticket system

If a resource has a ticket system for users to get support, use it instead of communicating by email. If such a system is in place, then the administrators running it are used to getting requests this way. If you email directly, you may not receive feedback in a timely manner, or the email might get lost.

### Specific Rules

Ultimately, it is very important to learn about the rules, practices, and etiquette for the resource that you are using and to follow them. Otherwise, you could lose access. Other users are also a great resource!
 

## Interacting with shared resources

Often you will need to use the command line to interact with a server from your personal computer. To do so on a Mac or a Linux computer, you can typically use the terminal program that is already on your computer. For PC or Windows computer users, you can use programs like [MobaXterm](http://mobaxterm.mobatek.net/).

If you wish to run a program with a graphical interface, then you might need to have a program to help you do so. On Macs, you can download [XQuartz](http://xquartz.macosforge.org/landing/). If you use MobaXterm on your PC or Windows computer, then you will already be set. Linux computers also typically should already have what you need.

If you are new to Unix commands check out this cheat sheet below.


```
## `google-chrome`, `chromium-browser` and `chrome` were not found. Try setting the `CHROMOTE_CHROME` environment variable to the executable of a Chromium-based browser, such as Google Chrome, Chromium or Brave or adding one of these executables to your PATH.
```

<iframe src="https://files.fosswire.com/2007/08/fwunixref.pdf" width="100%" height="400px" data-external="1"></iframe>


## Running Jobs

Typically a program is used to schedule jobs. Remember that jobs are the individual computational tasks that you ask the server to run. For example, this could be something as simple as moving large files from one directory to another, or as complex as running a complicated script on a file. 

Such job scheduling programs assign jobs to available node resources as they become available and if they have the required resources to meet the job. These programs have their own commands for running jobs, checking resources, and checking jobs. Remember to use the management system to run your jobs using the compute nodes not the login nodes (nodes for users to log in). There are often nodes set up for transferring files as well. 

In the case of the JHPCE, a program called Sun Grid Engine (SGE) is used, but there are others job management programs. See [here](https://jhpce.jhu.edu/orient/images/sge-orient.pdf) for more information on how people use SGE for the JHPCE shared resource.

### Specifying memory (RAM) needs

Often there is a default file size limit for jobs. For example, the JHPCE has a 10GB file size limit for jobs. When you have a job using a file that exceeds that limit, you may need to specify and set the file size accordingly for that job. As you may recall, if you are using whole genome files you are likely to exceed the default file limit size. 

In addition to the file size limit, you are often also given a default amount of RAM for your job as well. Again, you can typically run a job with more RAM if you specify. Similar to the file size limit, you will likely need to set the RAM that you will need for your job if it is above the default limit. This involves setting a lower and upper limit to the RAM that your job can use. If your job exceeds that amount of RAM it will be stopped. Typically people call stopping a job "killing" it. The lower and upper limit can be the same number.

How do you know how much RAM to assign to your job? Well, if you are performing a job with files that are two times the size of the file size default limit, then it might make sense to double the RAM you would typically use. **It's also a good idea to test on one file first if you are going to perform the same job on multiple files.** You can then assess how much RAM the job used. First, try to perform the job with lower limits, then progressively increase the size until you see that the job was successful and not killed for exceeding the limit. Keep in mind, however, how much RAM there is on each node. Remember, it is important not to ask for all the RAM on a single node or core on that node, as this will result in you hogging that node and other users will not be able to use RAM on that node or core on that node. Remember that you will likely have the option to use multiple cores. This can also help you to use less RAM across each core. For example, a job that needs 120GB of RAM could use 10 cores with 12 GB of RAM each.

Often there will be a limit for the number of jobs, the amount of RAM, and the number of cores that a single user can use beyond the default limits. This is to ensure that a user doesn't use too many resources causing others to not be able to perform their jobs. Check to see what these limits are, and then determine the appropriate way to contact to request for more. Again, communication standards and workflows may vary based on the resource.

### Checking status

It's also a good idea to check the status of your jobs to see if they worked or got killed. You can check for the expected file outputs or there are commands for the server management software that can help you check currently running jobs.

## Storage

Often you will be given a home directory which will likely be backed up. However, other storage directories often will not be. Be careful about where you store your data, as some directories might be for temporary use and get wiped to keep space available for others.

## Conclusion

We hope that this chapter has given you some more knowledge about why and how more traditional shared computing resources are shared.

In conclusion, here are some of the major take-home messages:

1) Shared resources like high performance computing clusters need regulations so that computing resources are shared fairly to allow everyone to get the most work done.
2) Paying attention to security is important to keep everyone's data and work on the server safe.
3) Although we provided general guidelines, there are likely to be specific guidelines for specific resources that you need to adhere to.
4) Often such resources have a communication process to avoid overloading resource administrators/mangers with too many requests. Be sure to follow the appropriate communication etiquette for the resources that you work with.
5) Although there are generally default limits for jobs, users can often consult with the appropriate communication infrastructure to ask to perform larger jobs.


