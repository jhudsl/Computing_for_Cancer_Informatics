




# Data Security

In this chapter we will discuss best practices for keeping your data safe and secure.

<img src="resources/images/08-Data_Security_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_gf5f8818810_1_171.png" title="Learning Objectives: 1.Recognize general informatics computing and data management platforms. 2.Be aware of specific genomics data management systems 3.Be aware of specific imaging data management systems  4.Be aware of specific clinical data management systems" alt="Learning Objectives: 1.Recognize general informatics computing and data management platforms. 2.Be aware of specific genomics data management systems 3.Be aware of specific imaging data management systems  4.Be aware of specific clinical data management systems" width="100%" style="display: block; margin: auto;" />

Data security involves protecting your data from human error, as well as from cybercriminals. Precious data needs to be protected from being corrupted (rendered unusable), being deleted, being misused, and being leaked to the public when the data is sensitive or private (as is the case with much of our clinical data)[@IBM_data_security].

# Data Security Strategies

There a several major strategies to achieve data security. We will cover the following 4 major categories, in part according to @IBM_data_security.

<img src="resources/images/08-Data_Security_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g1016753ce66_0_7.png" title="Major Data Security Methods: 1) Restricted access - minimizing access to only authorized users, 2) Data masking - removing/obscuring/changing values a) De-identification -concealing data that can be used to identify patients b) Data encryption - translating the data mathematically 3) Data erasure - fully deleting all traces of data from shared spaces, 4) Data resiliency - maintaining backups of the data and recovery strategies" alt="Major Data Security Methods: 1) Restricted access - minimizing access to only authorized users, 2) Data masking - removing/obscuring/changing values a) De-identification -concealing data that can be used to identify patients b) Data encryption - translating the data mathematically 3) Data erasure - fully deleting all traces of data from shared spaces, 4) Data resiliency - maintaining backups of the data and recovery strategies" width="100%" style="display: block; margin: auto;" />

## Data access

## Data masking

Encryption is actually just one of the more complex methods of a larger concept called data masking for protecting sensitive data. There are other methods for obscuring parts of the data besides the complexity of encryption, such as the following:

<img src="resources/images/08-Data_Security_files/figure-html//1B4LwuvgA6aUopOHEAbES1Agjy7Ex2IpVAoUIoBFbsq0_g1016753ce66_0_0.png" title="Data Masking Methods" alt="Data Masking Methods" width="100%" style="display: block; margin: auto;" />

### De-identification
https://www.hhs.gov/hipaa/for-professionals/privacy/special-topics/de-identification/index.html
https://opin.com/de-identify-health-information-phi-v2/


### Encryption

Encryption is one of the most well-known methods for keeping data safe. The process involves encoding or scrambling the data in a nonrandom format (we call this form of the data **encrypted**) that given the right instructions, a computer can reformat into the original form in a process called **decryption**. The instructions called the **key** are kept safe like a password and depending on the type of encryption, it can require quite a lot of computational power to decrypt the data. This protects the data because if a cybercriminal accesses the data or if the data is somehow made public when it shouldn't be, it will not be easily interpreted [@Forcepoint2018]. 


There are different methods for encrypting data. One common method is called asymmetric, which involves two keys, a **public key** and a **private key** [@IBM_encryption].

Users can get access to the public key to allow them to encrypt the data, while the private key remains private and is used to decrypt the data. This method is also called public-key encryption [@IBM_encryption].

Symmetric cryptography on the other hand uses **one** key for encryption and decryption. In systems that use this type of encryption, pairs of users will often be given their own key. The advantage of this system is that decryption is a bit faster, the keys are smaller, and it is generally less expensive to implement. If someone gains access to the key, however they can decrypt data or messages, and encrypt data or messages and appear as if they are the person that owns that key. So often the keys themselves are encrypted [@IBM_encryption].

Since symmetric decryption is faster, it is often used for transferring data or for large datasets.Common symmetric algorithms are [AES-128, AES-192, and AES-256](https://www.trentonsystems.com/blog/aes-encryption-your-faqs-answered) [@cyware_social_encryption].

Asymmetric encryption is regarded to be more secure, common algorithms included [RSA](https://simple.wikipedia.org/wiki/RSA_algorithm) and [DSA](https://en.wikipedia.org/wiki/Digital_Signature_Algorithm), and several [PKCS](https://en.wikipedia.org/wiki/PKCS) standards [@cyware_social_encryption].


These algorithms involve mathematical operations to encrypt the data. See this video for a simplified explanation and a suggestion for a video series if you want to learn more about how these encryption algorithms work:


<iframe src="https://www.youtube.com/embed/ZPXVSJnDA_A?start=459" width="100%" height="400px"></iframe>


## Data erasure

## Data resiliency

## Security in workflows
