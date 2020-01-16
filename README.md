# Drug Repurposing for Cancer - A Data Driven Approach

## Project coordinators: 
- [IBM Research](https://researcher.watson.ibm.com/researcher/view.php?person=us-ioana)
- [Cures Within Reach for Cancer](https://www.cwr4c.org/)

![Drug repurposing](https://github.com/JinjunXiong/TechTogether2020/blob/master/pills_banner.png 'Drug Repurposing')

## Project Context: Synthesizing scientific data on generic drugs for cancer treatment

Each year around the world, nearly 10 million people die from [cancer](https://www.cancerresearchuk.org/health-professional/cancer-statistics/worldwide-cancer) and the cost of cancer exceeds USD [$1 trillion](https://issuu.com/uicc.org/docs/wcls2014_economics_of_cancer_final?e=10430107/10454633). Finding new therapeutic uses for inexpensive generic drugs ("drug repurposing") can rapidly create affordable new treatments. Hundreds of non-cancer generic drugs have shown promise for treating cancer, but it is unclear which are the most worthwhile repurposing opportunities to pursue. Conducting randomized controlled trials to fully establish the efficacy of such drugs is highly expensive (in the order of 5-10 million of dollars), and such, prioritizing the most promissing drugs is crucial to reducing cost of cancer treatments. 

Scientific publications such as preclinical laboratory studies and small clinical trials contain evidence on generic drugs being tested for cancer use. For example, the [Repurposing Drugs in Oncology](http://www.redo-project.org/) (ReDO) project, through manually inspecting research articles indexed by PubMed, found anti-cancer evidence for more than 200 non-cancer generic drugs. However, manual review to identify and analyze potential evidence is time-consuming and intractable to scale. As PubMed indexes millions of articles and the collection is continuously updated, it is imperative to devise (semi)automated techniques to synthesize the existing evidence. Machine learning (ML)-powered evidence synthesis would provide a comprehensive and real-time view of drug repurposing data and enable actionable insights. 

We are currently collaborating on an ambitious initiative to synthesize the plethora of scientific and real-world data on non-cancer generic drugs to identify the most promising therapies to repurpose for cancer. At the moment, we are focusing on the key aspect of identifying and extracting relevant evidence from PubMed articles. If you are interested in reading more about our work, you can read a [short paper](https://arxiv.org/abs/1911.07819) on this topic. 

To be able to train machine learning algorithms to identify and extract relevant evidence from the scientific literature, decent size datasets of high quality are required. So far, we have been using in-house expertise to annotate scientific abstracts from PubMed. We are interested in scaling the annotations to a more diverse crowd that do not necessarily have a solid background in biology. This challenge is focused on this key problem. 

## TechTogether Challenge Brief Description: Tool for Evidence Annotation of Scientific Literature

**TL;DR:** We are asking the participants to design and develop an annotation tool that makes it easy to annotate scientific articles by a diverse crowd. The teams will compete by using each others' tools to annotated several scientific articles. The quality of the tool will be evaluated using a small subset of articles for which we provide ground truth. 

This challenge will be split into three parts, as follows:

1. Design and implement a tool for annotating scientific abstracts from PubMed. The key requirement of the tool is that it needs to make it easy to annotate scientific abstracts by a diverse crowd that do not necessarily have a solid background in biomed. We will explain in detail shortly, providing several examples, the type of annotations that have to be collected. 
2. The teams participating in the challenge will compete by using each others' tools and annotate several PubMed abstracts. 
3. The quality of the annotations collected will be assesed by the teams by programmatically comparing the annotated collected by their tools with the ground truth that we will provide. 

Bonus Problem: For those interested in an additional challenge, we are providing a small dataset with labels on whether the articles are of interest for our synthesis or not. The participants are asked to implement a model that, given an abstract, predicts whether the paper is of interest for our synthesis. We will explain all details below. 


## Challenge Timeline and Process Description
 

## Challenge Evaluation Criteria

## Annotation Description
