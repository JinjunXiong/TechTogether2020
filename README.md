# Drug Repurposing for Cancer - A Data Driven Approach

## Introduction
This project is designed for the [TechTogether Boston 2020](https://boston.techtogether.io) held from January 31 - Feb 2, 2020 in Agganis Arena, Boston University.This project is specifically designed for the [TechTogether Boston 2020](https://boston.techtogether.io),Boston's largest all-female, femme, and non-binary hackathon, held from January 31 - Feb 2, 2020 in Agganis Arena, Boston University.

If you are not clear about any particular concept as discussed below, please ask your technical mentors to help you. You can choose to finish the project using whatever programming language you are comfortable with, be it Python, Javascript, Go, R, Matlab, Mathematica, JAVA, C/C++, or whatever. 

![Drug repurposing](https://github.com/JinjunXiong/TechTogether2020/blob/master/pills_banner.png 'Drug Repurposing')

## Motivation: Synthesizing scientific data on generic drugs for cancer treatment

Each year around the world, nearly 10 million people die from [cancer](https://www.cancerresearchuk.org/health-professional/cancer-statistics/worldwide-cancer) and the cost of cancer exceeds USD [$1 trillion](https://issuu.com/uicc.org/docs/wcls2014_economics_of_cancer_final?e=10430107/10454633). Finding new therapeutic uses for inexpensive generic drugs ("drug repurposing") can rapidly create affordable new treatments. Hundreds of non-cancer generic drugs have shown promise for treating cancer, but it is unclear which are the most worthwhile repurposing opportunities to pursue. Conducting randomized controlled trials to fully establish the efficacy of such drugs is highly expensive (in the order of 5-10 million of dollars), and such, prioritizing the most promissing drugs is crucial to reducing cost of cancer treatments. 

Scientific publications such as preclinical laboratory studies and small clinical trials contain evidence on generic drugs being tested for cancer use. For example, the [Repurposing Drugs in Oncology](http://www.redo-project.org/) (ReDO) project, through manually inspecting research articles indexed by [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/), found anti-cancer evidence for more than 200 non-cancer generic drugs. However, manual review to identify and analyze potential evidence is time-consuming and intractable to scale. As [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) indexes millions of articles and the collection is continuously updated, it is imperative to devise (semi)automated techniques to synthesize the existing evidence. Machine learning (ML)-powered evidence synthesis would provide a comprehensive and real-time view of drug repurposing data and enable actionable insights. 

We are currently collaborating on an ambitious initiative to synthesize the plethora of scientific and real-world data on non-cancer generic drugs to identify the most promising therapies to repurpose for cancer. At the moment, we are focusing on the key aspect of identifying and extracting relevant evidence from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) articles. If you are interested in reading more about our work, you can read a [short paper](https://arxiv.org/abs/1911.07819) on this topic. 

To be able to train machine learning algorithms to identify and extract relevant evidence from the scientific literature, decent size datasets of high quality are required. So far, we have been using in-house expertise to annotate scientific abstracts from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/). We are interested in scaling the annotations to a more diverse crowd that do not necessarily have a solid background in biology. This challenge is focused on this key problem. 

## Challenge Description: Designing Best Tools for Evidence Annotation of Scientific Literature

This challenge will be split into three step as follows. We are asking participant teams to 

1. Design and develop a web-baseed annotation tool that makes it easy to annotate scientific articles by a diverse crowd. The scientific abstracts are obtained from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/). The key requirement of the web tool is that it needs to make it easy to annotate scientific abstracts by a diverse crowd that do not necessarily have a solid background in biomed. We will explain in detail shortly, providing several examples, the type of annotations that have to be collected. The organizer will assign each team a set of PubMed scientific article abstracts to be used for testing in step 2 below. The first step of the project will need to be done prompty by **Friday 1 pm (EST), Feb 1st, 2020** without incurring penalty. This is essential as the Step 2 will depend on the Step 1 outcome.
2. Use each others' tools developed in Step 1 to annotated several PubMed scientific article abstracts, and rate the quality of the tools (metrics to be described below) each team is assigned to use (in other words, teams will rate each other's tools and compete against each other). The organizer will assign each team the annotation tools developed by other teams to use. 
3. Evaluate the quality of annotation results from Step 2 from all annotators by programmatically comparing against a small subset of articles for which we provide ground truth.  


Bonus Problem: For those interested in an additional challenge, we are providing a small dataset with labels on whether the articles are of interest for our synthesis or not. The participants are asked to implement a model that, given an abstract, predicts whether the paper is of interest for our synthesis. We will explain all details below. 


## Challenge Timeline and Process Description
 

## Challenge Evaluation Criteria

## Annotation Description

## Acknowledgements:
- [IBM Research](https://researcher.watson.ibm.com/researcher/view.php?person=us-ioana)
- [Cures Within Reach for Cancer](https://www.cwr4c.org/)
