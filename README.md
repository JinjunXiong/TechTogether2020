# Drug Repurposing for Cancer - A Data Driven Approach

## TechTogether 2020 Project
This project is specifically designed for the [TechTogether Boston 2020](https://boston.techtogether.io), Boston's largest all-female, femme, and non-binary hackathon, held from January 31 - Feb 2, 2020 in Agganis Arena, Boston University.

If you are not clear about any particular concept as discussed below, please ask your technical mentors to help you. You can choose to finish the project using whatever programming language you are comfortable with, for example Python, Javascript, Go, R, Matlab, Mathematica, JAVA, C/C++, and any technologies (Amazon AWS, IBM Cloud Fuctions, Google Cloud, etc.). 

![Drug repurposing](https://github.com/JinjunXiong/TechTogether2020/blob/master/pills_banner.png 'Drug Repurposing')

## Motivation: Synthesizing scientific data on generic drugs for cancer treatment

Each year around the world, nearly 10 million people die from [cancer](https://www.cancerresearchuk.org/health-professional/cancer-statistics/worldwide-cancer) and the cost of cancer exceeds USD [$1 trillion](https://issuu.com/uicc.org/docs/wcls2014_economics_of_cancer_final?e=10430107/10454633). Finding new therapeutic uses for inexpensive generic drugs ("drug repurposing") can rapidly create affordable new treatments. Hundreds of non-cancer generic drugs have shown promise for treating cancer, but it is unclear which are the most worthwhile repurposing opportunities to pursue. Conducting randomized controlled trials to fully establish the efficacy of such drugs is highly expensive (in the order of 5-10 million of dollars), and such, prioritizing the most promissing drugs is crucial to reducing cost of cancer treatments. 

Scientific publications such as preclinical laboratory studies and small clinical trials contain evidence on generic drugs being tested for cancer use. For example, the [Repurposing Drugs in Oncology](http://www.redo-project.org/) (ReDO) project, through manually inspecting research articles indexed by [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/), found anti-cancer evidence for more than 200 non-cancer generic drugs. However, manual review to identify and analyze potential evidence is time-consuming and intractable to scale. As [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) indexes millions of articles and the collection is continuously updated, it is imperative to devise (semi)automated techniques to synthesize the existing evidence. Machine learning (ML)-powered evidence synthesis would provide a comprehensive and real-time view of drug repurposing data and enable actionable insights. 

We are currently collaborating on an ambitious initiative to synthesize the plethora of scientific and real-world data on non-cancer generic drugs to identify the most promising therapies to repurpose for cancer. At the moment, we are focusing on the key aspect of identifying and extracting relevant evidence from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) articles. If you are interested in reading more about our work, you can read a [short paper](https://arxiv.org/abs/1911.07819) on this topic. 

To be able to train machine learning algorithms to identify and extract relevant evidence from the scientific literature, decent size datasets of high quality are required. So far, we have been using in-house expertise to annotate scientific abstracts from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/). We are interested in scaling the annotations to a more diverse crowd that do not necessarily have a solid background in biology. This challenge is focused on this key problem. 

## Challenge Description: Designing Best Tools for Evidence Annotation of Scientific Literature

This challenge will be split into three step as follows. We are asking the participant teams to execute on the following steps:

1. Design and develop a web-baseed annotation tool that makes it easy to annotate scientific articles by a diverse crowd. The scientific abstracts are obtained from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/). A subset used for this exercise will be provided, so no need to acces PubMed. The key requirement of the web tool is that it needs to make it easy to annotate scientific abstracts by a diverse crowd that do not necessarily have a solid background in biomed. We will explain in detail shortly, providing several examples, the type of annotations that have to be collected. The organizer will assign each team a set of PubMed scientific article abstracts to be used for testing in step 2 below. The first step of the project will need to be done prompty by **Saturday 4 pm (EST), Feb 1st, 2020** without incurring penalty. This is essential as subsequent steps require this first step to be completed.
2. Use each others' tools developed in Step 1 to annotate the provided PubMed scientific abstracts, and rate the quality of the tools (metrics to be described below). Each team will be assigned to use a different team's tool, so this part of the project is a mini-competition among teams. We expect all teams to finish this step by **Saturday 6pm (EST), Feb 1st, 2020** such that there is sufficient time to analyze the results and prepare your submissions.
3. Evaluate the quality of annotation results from Step 2 from all annotators by programmatically comparing against a the ground truth, which will be provided. Based on the results you obtain, discuss the efficiency of the tool and draw conclusions on what could improve.


Bonus Problem: For those interested in an additional challenge, we are providing a small dataset with labels on whether the articles are of interest for our synthesis or not. The participants are asked to implement a model that, given an abstract, predicts whether the paper is of interest for our synthesis. We will explain all details below. 


## Challenge Timeline and Process Description
 In this section we clarify the process and the timeline. Please consult with your tech mentors at any point if you have questions. Don't be shy and don't wait. Rule of thumb: if it takes more than 15 mins to figure out, ask for help.

 Please note the general schedule on the hackathon's webpage. These steps are only the steps specific to our project. 

 1. Friday night, after project pitch, we're expecting the participant teams interested in executing on the project to submit a issue to this github repo with the name of the team in the title of the issue. The body of the issue should contain the name of the participants and the github repository where all code, results and analysis will be deposited. We expect this step to be completed by **Saturday 9am, Feb 1st, 2020**. At this point, we will distribute about 50 abstracts that need to be included in the experiments. Also we will distribute a set of 100 abstracts for those who want to work on the bonus component. 
 2. By **Saturday 2pm, Feb 1st, 2020**, the organizers will match teams for the competition part. Each team will have a different team assigned. They have to make sure the teams communicate to understand how to use the annotation tools.
 3. Teams are expected to work on the annotation tools until 4pm. By that point, all teams should know how to access the other team's tool to provide annotations. We count on your honesty! Please do a great job when providing annotations. We'll be taking into account your performance when ranking the submissions. *Between 4pm and 6pm*, we expect the teams to provide annotations. 
4. By **Saturday 6pm, Feb 1st, 2020**, teams are expected to complete the annotation period and they should be ready to analyize the results. 
5. By **Sunday 8am, Feb 2nd, 2020**, teams will be working on analyzing the results of the annotation tools, propose modifications and comment on the efficiency of their tool. All this information can be upload it in the issue belonging to the team. 
6. **Sunday 8am, Feb 2nd 2020**, we will clone all the repositories from the team. We will use the information in the repositories and in the issue to estimate the quality of the submission. 


## Challenge Evaluation Criteria
All the parts of the challenge will be taken into consideration when evaluating the solutions. We will analyze the tool design, the quality of the annotations that were received, the quality of the annotations that were provided, the analysis of the results and also the qualitative analysis of the tool and planned features, proposed changes. 

## Annotation Description
In this section we describe what makes an article interesting for our study and once such an abstract is identified, what type of information we need to collect to make possible to automate the synthesis of generic drug efficacy for cancer.


## Acknowledgements:
- [IBM Research](https://researcher.watson.ibm.com/researcher/view.php?person=us-ioana)
- [Cures Within Reach for Cancer](https://www.cwr4c.org/)
