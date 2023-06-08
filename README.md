# Research-Paper-Summarization


## Introduction
We aim to create a system to summarize and simplify academic research papers which we hope can be extended to academic writing of any kind. Reading research papers is a skill that has to be learnt. The task is daunting and time consuming for new academics. Academics often spend hours pouring over research papers during the course of their research. We aim to optimize this by providing academics and researchers concise and informative summaries of papers. This can be extended to to simplify all manners of technical documentation, such as medical reports, audit reports, industrial product manuals, etc., based on the information used to train our system. We forecast that a successful summarization algorithm can reduce countless human work hours in large volumes thus opening avenue to new research and developments. Laypeople, hobbyists, people who do not have years of education in a particular field would be able to understand concepts and implement them if they choose to, promoting interdisciplinary progress. 

## Project
### Extractive Approach
While our main goal was to make summaries of academic papers, we experimented with different methods to achieve our results. We used a dataset created by Ed Collins, et al [1]. which was mined from ScienceDirect and contained summaries, called “Highlights”, penned by the authors themselves. Our initial approach was to score each sentence based on the words that overlapped between the main body of the paper and the author generated summaries. The top “n” sentences with the highest scores were picked as summary sentences. 

#### Generated Extractive Summary
```
[' No such relationship was observed in the left hand',
 ' The measurement was performed first on the right and then the left hand',
 ', 2004; Solovieva etal',
 ' Dentists heavily utilize the thumb, index, and middle fingers in precision gripping in the right (or dominant) hand, while the left hand remains static for supportive work tasks']
```
#### Author Generated Highlights
```
['The relationship of task variation during dental work history with pinch grip strength among dentists was investigated',
 ' The dentists with the most hand-loading tasks were at an increased risk of low pinch grip strength',
 ' It is advisable among dentists to perform as diverse work tasks as possible to reduce the risk of decreased pinch grip strength',
 '']
```

## Summary
There are state of the art methods, such as transformers, which do a good job at summarization but none of which have been applied to the domain of research paper summarization. Our task was to summarize research papers using analytical method, extractive and we have tried to measure performances of the tasks. We mined research papers under the topic of Computer Science from the ScienceDirect website using the method provided in the research paper “A Supervised Approach to Extractive Summarisation of Scientific Papers”[1]. We spent quite some time processing the data as the output from the mining algorithm was messy. We created two models for extractive method, and we trained and tested them. The faults in our models were substantially different. While our extractive model produced grammatically coherent but irrelevant summaries and Also our models did not perform well, more training time and computational power would definitely improve it. 

