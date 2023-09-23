# Summarise Schneier 2015: Applied Cryptography: 2.3 One-Way Functions 

The article discusses the concept of one-way functions, which play a crucial role in public-key cryptography. One-way functions are relatively simple to compute in one direction but extremely difficult to reverse. In other words, it's easy to calculate the output of a function given an input, but it's nearly impossible to determine the input when only the output is known. This property is essential for cryptographic protocols.

To illustrate the concept of one-way functions, the article uses the example of breaking a plate into pieces. It's easy to shatter a plate, but reassembling it from the fragments is exceedingly challenging.

However, the article acknowledges that there is no mathematical proof of the existence of one-way functions, nor concrete evidence of their construction. Nevertheless, many functions appear to exhibit one-way behavior, making them valuable tools in cryptography.

The article also introduces the idea of trapdoor one-way functions, which are a specialized type of one-way function with a secret trapdoor. These functions are easy to compute in one direction and hard to compute in the reverse direction, except when you possess the secret information (the trapdoor). With this secret, you can easily compute the function in the reverse direction.

An analogy is made to taking apart and reassembling a watch. Disassembling a watch into tiny pieces is straightforward but putting it back together is challenging. However, having access to the assembly instructions (the secret information) makes the reassembly process much simpler.

In summary, one-way functions are fundamental components of public-key cryptography, characterized by their ease of computation in one direction and difficulty in the reverse direction. Trapdoor one-way functions introduce the concept of secret information that simplifies the reverse computation. While their existence is not definitively proven, they are essential for secure encryption and cryptographic applications.

# Summarise Schneier 2015: Applied Cryptography: 2.4 One-Way Hash Functions

The article discusses the significance of one-way hash functions in modern cryptography, emphasizing their role as a foundational element in various protocols. These functions are also known by several names, such as compression function, message digest, fingerprint, cryptographic checksum, message integrity check (MIC), and manipulation detection code (MDC).

A one-way hash function is a fundamental concept in computer science, defined as a function that takes a variable-length input string (pre-image) and converts it into a fixed-length output string (hash value). An example of a simple hash function is one that computes the XOR of all input bytes to create the hash value. The primary purpose of hash functions is to create a unique fingerprint for the pre-image, indicating whether a given candidate pre-image matches the actual one. While hash functions are typically many-to-one, they provide a reasonable level of certainty about the accuracy of the comparison.

Crucially, a one-way hash function operates in a single direction: it is easy to compute a hash value from a pre-image, but exceedingly challenging to reverse the process and generate a pre-image that produces a specific hash value. Unlike simpler hash functions, a good one-way hash function is collision-free, meaning it's extremely difficult to find two different pre-images that produce the same hash value.

Importantly, the security of a one-way hash function lies in its one-wayness, and the function itself is public with no inherent secrecy. Changing a single bit in the pre-image results in, on average, half of the bits in the hash value changing as well. Given a hash value, it is computationally infeasible to determine the original pre-image that produced it.

The article provides an illustrative example of using one-way hash functions for file fingerprinting. To verify if someone possesses a specific file without them sending it, one can request the hash value of the file. If the sender provides the correct hash value, it's highly likely that they have the corresponding file. This method is particularly useful in financial transactions to prevent unauthorized changes to transaction amounts in a network.

Additionally, the article introduces the concept of Message Authentication Codes (MACs), which are one-way hash functions enhanced with a secret key. MACs operate on both the pre-image and the key, ensuring that only someone with the key can verify the hash value. MACs can be created from hash functions, block encryption algorithms, or specialized MAC algorithms.

In summary, one-way hash functions are essential in modern cryptography for their ability to generate unique fingerprints of data, and they play a crucial role in verifying data integrity and security in various applications, including financial transactions. Message Authentication Codes further enhance security by introducing a secret key into the hash computation process.

### Reference https://learning.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/10_chap02.html#chap02-sec003

# Summarise Nicolas Särökaari Presentation in 2018

The speaker, Nicolas Särökaari, discusses the topic of email phishing in his presentation. He introduces himself as a security professional working at Silverskin, and his interest lies in breaking security measures, watching movies, and drinking coffee.

He explains the concept of phishing, which involves sending emails that appear to come from legitimate sources with the aim of gaining unauthorized access to sensitive data, personal information, passwords, or an organization's internal network. Phishing emails may contain malicious links or attachments designed to deceive users.

Nicolas delves into why people click on phishing links, citing a 2016 study that found curiosity to be a significant motivator. People are more likely to click on links out of curiosity, expectations, or if they think they know the sender.

He discusses various protection mechanisms, such as SPF (Sender Policy Framework), DKIM (DomainKeys Identified Mail), and DMARC (Domain-based Message Authentication, Reporting, and Conformance), which organizations can implement to mitigate phishing threats.

Nicolas also touches on ways to bypass these protection mechanisms, emphasizing the importance of securing infrastructure, regularly updating servers and workstations, and educating users about phishing risks.

He presents several phishing scenarios, including emails about package deliveries, password leaks, and file sharing, illustrating how attackers can trick users into clicking links or submitting their credentials.

Nicolas concludes by highlighting the challenges in getting users to report phishing attempts and advises skepticism when receiving emails from unknown sources or with suspicious content.

Overall, Nicolas Särökaari's presentation provides insights into the world of email phishing, its effectiveness, and ways to protect against it.

### Reference https://www.youtube.com/watch?v=m9YFJGSHYtY


