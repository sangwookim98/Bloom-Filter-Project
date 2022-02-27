# MinHash Project: Plagarism Detector
Plagarism Detector code by implementing technique of MinHashing. Plagarism of a document can be determined by Jaccard's Measure after comparing two documents. 


##### MinHash
Commonly used technique in Data Mining, MinHashing is a technique where it would calculate similarities of two sets. MinHash is a very efficient way of comparing a large number of doucments because by using a MinHash signature, it would not only decrease the runtime complexity by a large amount, but it would also allow the comparison of the sets to be easily implemented rather than having to compare each single a lot of times within a large collection of documents given. 

#### Jaccard's Measure
Jaccard's Measure is the resemblence of two sets of arbitrary sizes as a result of comparing two MinHash-ed documents. 

### Process of Plagarism Detector:

1. Filter out each document by elimating all StopWords such as "I", "to", "with", "the", "for", "of", and any other words that do not give or influence the overall meaning of the passage. 

2. Breakdown of each documents into shingles, or groups of consecutive words in the exact order these words appear in the .txt files. 

3. Store minimum hash value of each shingles per hash function. If there's k-number of hash functions, it would storea minimum hash value for a total of k times. 

4. Compare shingles of each documents and find similarity using Jaccard's Measure. The higher the measure, the more likely the document is plagarized. 


### Purpose
The purpose of this project is to get a better understanding of probability, and gain an insight into how simiarity of two sets work. 
