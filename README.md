# Drug Repurposing for Cancer - A Data Driven Approach

## TechTogether 2020 Project

[IBM Research](https://research.ibm.com/) in collaboration with [Cures Within Reach for Cancer](https://www.cwr4c.org/) is on an ambitious initiative to automatically analyze and mine the plethora of scientific publications and real-world data on non-cancer generic drugs to identify the most promising therapies to repurpose for cancer treatment.

In this year's IBM TechTegether Challenge, we ask you to join us to tackle this grand challenge together. As an innovative developer and out-of-the-box thinker, you are asked to develop a scalable and easy-to-use automation tool in the quest of analyzing scientific publications and data on generic drugs for cancer treatments.

You will learn what type of data needs to be collected on drugs and cancers from scientific papers to make it possible to automatically extract useful and insightful information, and how your tools developed through this IBM TechTegether Challenge will help us achieve such a goal with more accurate labeled data. You will even get a chance to use the tools developed by other teams (or, equivalently, let other teams use your tools) to see how your efforts can make a difference in collecting useful data, and finally programmatically measure the quality of the data you collect. For those who would like to take on an even bigger challenge, we have something extra for you to flex your machine learning and AI brain muscles.


This project is specifically designed for the [TechTogether Boston 2020](https://boston.techtogether.io), Boston's largest all-female, femme, and non-binary hackathon, held from January 31 - Feb 2, 2020 in Agganis Arena, Boston University.

If you are not clear about any particular concept as discussed below, please ask your technical mentors to help you. You can choose to finish the project using whatever programming language you are comfortable with, for example Python, Javascript, Go, R, Matlab, Mathematica, JAVA, C/C++, and any technologies (Amazon AWS, IBM Cloud Functions, Google Cloud, etc.). 

![Drug repurposing](https://github.com/JinjunXiong/TechTogether2020/blob/master/pills_banner.png 'Drug Repurposing')

## Motivation: Synthesizing scientific data on generic drugs for cancer treatment

Each year around the world, nearly 10 million people die from [cancer](https://www.cancerresearchuk.org/health-professional/cancer-statistics/worldwide-cancer) and the cost of cancer exceeds USD [$1 trillion](https://issuu.com/uicc.org/docs/wcls2014_economics_of_cancer_final?e=10430107/10454633). Finding new therapeutic uses for inexpensive generic drugs ("drug repurposing") can rapidly create affordable new treatments. Hundreds of non-cancer generic drugs have shown promise for treating cancer, but it is unclear which are the most worthwhile repurposing opportunities to pursue. Conducting randomized controlled trials to fully establish the efficacy of such drugs is expensive (in the order of 5-10 million of dollars), and such, prioritizing the most promising drugs is crucial to reducing the cost of cancer treatments. 

Scientific publications such as preclinical laboratory studies and small clinical trials contain evidence on generic drugs being tested for cancer use. For example, the [Repurposing Drugs in Oncology](http://www.redo-project.org/) (ReDO) project, through manually inspecting research articles indexed by [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/), found anti-cancer evidence for more than 200 non-cancer generic drugs. However, manual review to identify and analyze potential evidence is time-consuming and intractable to scale. As [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) indexes millions of articles and the collection is continuously updated, it is imperative to devise (semi)automated techniques to synthesize the existing evidence. Machine learning (ML)-powered evidence synthesis would provide a comprehensive and real-time view of drug repurposing data and enable actionable insights. 

We are currently collaborating on an ambitious initiative to synthesize the plethora of scientific and real-world data on non-cancer generic drugs to identify the most promising therapies to repurpose for cancer. At the moment, we are focusing on the key aspect of identifying and extracting relevant evidence from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/) articles. If you are interested in reading more about our work, you can read a [short paper](https://arxiv.org/abs/1911.07819) on this topic. 

To be able to train machine learning algorithms to identify and extract relevant evidence from the scientific literature, decent size datasets of high quality are required. So far, we have been using in-house expertise to annotate scientific abstracts from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/). We are interested in scaling the annotations to a more diverse crowd that do not necessarily have a solid background in biology. This challenge is focused on this key problem. 

## Challenge Description: Designing Best Tools for Evidence Annotation of Scientific Literature

This challenge will be split into three steps as follows. We are asking the participant teams to execute on the following steps:

1. Design and develop a web-based annotation tool that makes it easy to annotate scientific articles by a diverse crowd. An annotation tool is a web-based interface that, in our case, displays a piece of text and asks several questions to be answered with excerpts from the text or by underlining excerpts directly in the text. In this challenge, we work with scientific abstracts that are obtained from [PubMed](https://www.ncbi.nlm.nih.gov/pubmed/). A subset used for this exercise will be provided, so no need to access PubMed. The key requirement of the web tool is that it needs to make it easy to annotate scientific abstracts by a diverse crowd that do not necessarily have a solid background in biomedical research. We will explain in detail shortly, providing several examples, the type of annotations that have to be collected. The organizer will assign each team a set of PubMed scientific article abstracts to be used for testing in step 2 below. The first step of the project will need to be done promptly by **Saturday 4 pm (EST), Feb 1st, 2020** without incurring penalty. This is essential as subsequent steps require this first step to be completed.
2. Use each others' tools developed in Step 1 to annotate the provided PubMed scientific abstracts, and rate the quality of the tools (metrics to be described below). Each team will be assigned to use a different team's tool, so this part of the project is a mini-competition among teams. We expect all teams to finish this step by **Saturday 6pm (EST), Feb 1st, 2020** such that there is sufficient time to analyze the results and prepare your submissions.
3. Evaluate the quality of annotation results from Step 2 from all annotators by programmatically comparing against the ground truth, which will be provided. Based on the results you obtain, discuss the efficiency of the tool and draw conclusions on what could improve.


Bonus Problem: For those interested in an additional challenge, we are providing a small dataset with labels on whether the articles are of interest for our synthesis or not. The participants are asked to implement a model that, given an abstract, predicts whether the paper is of interest for our synthesis. We will explain all details below. 


## Challenge Timeline and Process Description
 In this section we clarify the process and the timeline. Please consult with your tech mentors at any point if you have questions. Don't be shy and don't wait. Rule of thumb: if it takes more than 15 mins to figure out, ask for help.

 Please note the general schedule on the hackathon's webpage. These steps are only the steps specific to our project. 

 1. Friday night, after project pitch, we're expecting the participant teams interested in executing on the project to submit an issue to this GitHub repo with the name of the team in the title of the issue. The body of the issue should contain the name of the participants and the GitHub repository where all code, results and analysis will be deposited. We expect this step to be completed by **Saturday 9am, Feb 1st, 2020**. At this point, we will distribute about 50 abstracts that need to be included in the experiments. Also we will distribute a set of 100 abstracts for those who want to work on the bonus component. 
 2. By **Saturday 2pm, Feb 1st, 2020**, the organizers will match teams for the competition part. Each team will have a different team assigned and they will use the tool produced by the assigned team to fill in annotations starting at **4pm on Saturday, Feb 1st 2020**. The teams have to communicate to understand how to use each others' annotation tools.
 3. Teams are expected to work on the annotation tools until 4pm. By that point, all teams should know how to access the other team's tool to provide annotations. We count on your honesty! Please do a great job when providing annotations. We'll be taking into account your performance when ranking the submissions. **Between 4pm and 6pm**, we expect the teams to provide annotations. 
4. By **Saturday 6pm, Feb 1st, 2020**, teams are expected to complete the annotation period and they should be ready to analyze the results. 
5. By **Sunday 8am, Feb 2nd, 2020**, teams should have completed analyzing the results of the annotation tools, propose modifications and comment on the efficiency of their tool. All this information can be uploaded to the issue belonging to the team. 
6. **Sunday 8am, Feb 2nd 2020**, we will clone all the repositories from the team. We will use the information in the repositories and in the issue to estimate the quality of the submission. 


## Challenge Evaluation Criteria
All the parts of the challenge will be taken into consideration when evaluating the solutions, as follows:
- Tool design: how easy it is to use, how straightforward it is to provide the annotations, assuming a non-biomedical background
- Quality of the collected annotations: compared to the ground truth, how accurate are the annotations that were collected with the tool
- Quality of the provided annotations: compared to the ground truth, how accurate are the annotations that are provided by the team
- Annotation analysis: was the comparison with the ground truth properly performed, is the analysis thorough
- Overall conclusions: are there any important take-aways in the qualitative analysis of the tool and planned features, proposed changes. 

## Annotation Guidelines
In this section we describe what makes an article interesting for our study and once such an abstract is identified, what type of information we need to collect to make it possible to automate the synthesis of generic drug efficacy for cancer. We will only be working with abstracts of articles, not the full texts.

The first task is to determine if any specific article is relevant to our work and should be included for future consideration. In a nutshell, we are interested in scientific abstracts that discuss the results of a non-cancer generic drug when tested as an intervention for cancer. Note the abstracts you will be using in this project will be provided. Also, for simplicity, the generic drugs discussed in each abstract will be provided as well. In addition, we are interested only in the abstracts that mention results at the *phenotype level* with respect to the cancer under consideration. Such results are directly associated with the cancer and they can generally be used to understand the efficacy of the drug in treating the cancer. Some of the medical terms used to describe such phenotypic outcomes include, but are not limited to: survival, tumor growth/reduction, apoptosis, metastasis, angiogenesis, cell proliferation, progression of disease, partial/complete response.


Some of the common scientific abstracts that discuss generic drugs and cancer but are **not** relevant for our use case often fit in one of the following categories:
- The abstract discusses an intervention of a generic drug for cancer, but it does not present direct measurements of the effect on cancer (e.g., no phenotypic outcomes are reported). Such papers can, for example, discuss the mechanism by which the drug affects the cancer; or they discuss some intermediate effect such as on immune cells (which may fight cancer).
- The abstract discusses using generic drugs to treat side effects of cancer.
- The abstract describes drugs tested to alter the risk of developing cancer.
- The abstract describes a study of tumors that are not cancerous.

Once an abstract is deemed as relevant for our collection, we are required to collect the following information:
- the generic drug
- the cancer type
- the therapeutic association
- the study type

The therapeutic association refers to the way the drug influences the cancer and can take one of the following values:
- `effective`: the drug helped treat the cancer (e.g., reduced the tumor size)
- `detrimental`: the drug made the cancer worse (e.g., caused the cancer to grow)
- `no effect`: the drug did not have a perceived effect on the cancer
- `inconclusive`: the results are mixed and no conclusion can be drawn.

The type of study refers to the type of experiments that were performed. This label can take one of the following values:
- `pre-clinical in-vivo`: experiments were done in animal models such as mice
- `pre-clinical in-vitro`: experiments are done with cultures of cancer cells
- `clinical trial`: experiments were done on patients in a clinical trial setting, the drug is used as an intervention for cancer
- `case report`: a detailed report of the symptoms, signs, diagnosis, treatment, and follow-up of an individual patient
- `observational study`: a study in which individuals are observed or certain outcomes are measured; no attempt is made to affect the outcome (for example, no treatment is given); these are not experiments, they are usually analysis of existing experiments and their results
- `other`: none of the above.

For the cases in which there are several generic drugs and/or cancers being discussed, you can select only one *(drug, cancer)* pair and provide the annotations with respect to the selected combination.

### Annotation Examples

#### Annotation Format

The tool should store the annotations in a tsv file (tab separated file) with the following header that specifies its fields:

`PubMedID   Title   Abstract    Relevant    Drug    Cancer  Therapeutic association     Study type`

Note that the PubmedID, Title and Abstract will be provided, the tool is supposed to collect the rest. The field `Relevant` can take only values `0` or `1`. The rest of the fields are collected only when an abstract is deemed relevant (i.e., the value of the `Relevant` field is `1`). Also note that for the therapeutic association and the study type, only the values mentioned in the previous section are allowed (see previous section, the values are in red). 

#### Example 1

```
PubMed ID: 15105045
Title: Potentiated anticancer effects on hepatoma cells by the retinoid adapalene.

Abstract: Retinoids can block cell proliferation and induce apoptosis in tumor cells. The antitumoral effect of synthetic retinoids like Adapalene (ADA) on hepatoma cells
(HepG2, Hep1B) was investigated. Cell proliferation was assessed by measuring DNA synthesis and apoptosis by flow cytometry and immunocytochemistry. Cell cycle- and 
apoptosis-associated proteins were semi-quantified by Western Blotting and breakdown of mitochondrial membrane potentials was detected by JC-1 staining. ADA at 10(-4)M 
efficiently induced apoptosis, reaching 61.7% in HepG2 and 79.1% in Hep1B after 72 h incubation. This was accompanied by up-regulation of pro-apoptotic bax and caspase 3, 
while bcl-2 was down-regulated, shifting the bax/bcl-2 ratio to >2.3 in hepatoma cells. ADA inhibits hepatoma cell growth in vitro and is a powerful inducer of hepatoma cell 
apoptosis.

Drugs: [Adapalene]
```

Relevant: 1 -> The article presents research that directly tests the effect of retinoid Adapalene on hepatoma cells. The phenotypic effect tested here is the apoptosis of tumor cells and blockage of cell proliferation. 
Drug: Adapalene
Cancer: Hepatoma
Therapeutic Effect: effective -> can block hepatoma cell growth and induces cell apoptosis
Study Type: preclinical in vitro -> no animal specified, no patient, the reserach presented here works directly with cells.


#### Example 2
```
PubMedID: 27465514
Title: The aqueous extract of cinnamon bark ameliorated cisplatin-induced cytotoxicity in vero cells without compromising the anticancer efficiency of cisplatin.

Abstract: AIM: Cis-diammine dichloroplatinum (CDDP) is one of the most important chemotherapeutic agents for cancer treatment. Nonetheless, its notable side effect, 
nephrotoxicity, undermines its clinical use. The current study was undertaken to evaluate the protective potential of the aqueous extract (AEC) of Cinnamomum cassia 
(cinnamon) against the cytotoxic effect of CDDP in vitro and to elaborate the molecular mechanism underlying protection. METHODS: MTT assay was performed to assess viability 
of the normal kidney Vero cells treated with CDDP and/or AEC. Cells were stained with Coomassie blue, acridine orange and ethidium bromide to highlight morphological 
features of apoptosis. Caspase-3 activity, DNA fragmentation and reactive oxygen species (ROS) level were monitored to assess biochemical hallmarks of apoptosis. 
Quantitative RT-PCR and Western blot analyses were performed to elucidate expression of cellular molecules underlying the protective potential of AEC. RESULTS: CDDP-treated 
Vero cells exhibited hallmarks of apoptosis; these hallmarks were significantly suppressed in the presence of AEC. AEC did not alter activity of CDDP-induced cytotoxicity of 
breast and liver cancer cells. AEC treatment of Vero cells prevented CDDP-induced increased expression of mitochondrial Bax protein, release of mitochondrial cytochrome c, 
caspase-3 activation, DNA fragmentation and generation of ROS. AEC up-regulated expression of the cytoprotective gene (heme oxygenase (HO)-1). CONCLUSION: These findings 
suggest AEC has protective effects against CDDP-induced toxicity via preventing the activation of various cellular mechanisms mediating apoptotic cell death, without 
compromising the anticancer efficiency of CDDP. Thus, cinnamon may represent one of the most feasible ways to reduce the risk of CDDP-induced toxicity.

Drugs: [cinnamon bark]
```

This abstract is not relevant for our purposes. It discusses an intervention for a side effect of one of the anti-cancer drugs.

#### Example 3
```
PubMedID 22733095
Title: Highly sulfated chondroitin sulfates, a novel class of prognostic biomarkers in ovarian cancer tissue.
Abstract: OBJECTIVE: Clinical decision making in ovarian cancer needs new (prognostic) biomarkers. Although the search for biomarkers has traditionally focused on tumor 
cells, their surrounding contains important information as well. Glycosaminoglycans, heterogeneous polysaccharides which are abundantly present in the stromal compartment, 
are indicated in several pathological processes including cancer. In this study we investigated a specific glycosaminoglycan motif (4,6-disulfated chondroitin sulfate) for 
its potential as a prognostic biomarker in ovarian cancer. METHODS: 4,6-Disulfated chondroitin sulfate presence was studied immunohistochemically using the single chain 
antibody GD3G7 on 148 ovarian tumors including benign and malignant tumors, and tumors with low malignant potential. For comparative purposes p53 and Ki-67 were evaluated. 
X2 tests, univariate and multivariate Cox proportional hazards analyses were applied for statistical analysis. RESULTS: The stroma of malignant tumors showed significantly 
increased expression of 4,6-disulfated chondroitin sulfate (GD3G7 epitope) compared with benign tumors and tumors with LMP (p-values<0.000 and 0.002, respectively). 
Expression of GD3G7 in malignant tumors was significantly correlated with serous subtype, high tumor grade, advanced FIGO-stage and high CA-125 levels. In patients with 
advanced FIGO stage GD3G7 expression was significantly correlated with incomplete debulking and good response to platinum-based chemotherapy. GD3G7 surpassed both p53 and 
Ki-67 in statistical analysis. Multivariate survival analysis revealed GD3G7 expression as an independent predictor for progression free survival. CONCLUSION: 
Glycosaminoglycan motifs may form a new class of biomarkers for (ovarian) cancer, as indicated here for the GD3G7 epitope. Expression of GD3G7 may contribute in therapeutic 
decision making and constitutes a potential biomarker for poor prognosis.

Drugs: [chondroitin sulfates]
```
This abstract is not relevant since it discussing a drug as a biomarker for cancer and the drug is not used as treatment.

#### Example 4

```
PubMedID: 15998950
Title: A large cohort study of aspirin and other nonsteroidal anti-inflammatory drugs and prostate cancer incidence.

Abstract: BACKGROUND: Use of aspirin and other nonsteroidal anti-inflammatory drugs (NSAIDs) has consistently been associated with a reduced risk of colon cancer. Recent 
epidemiologic studies have suggested that the use of NSAIDs, particularly aspirin, may also be associated with a reduced risk of prostate cancer, but the evidence remains 
limited. METHODS: We examined the association between NSAID use and prostate cancer incidence among 70 144 men in the American Cancer Society's Cancer Prevention Study II 
Nutrition Cohort. Information on NSAID use was obtained from a questionnaire completed at study enrollment in 1992-1993 and was updated using follow-up questionnaires in 
1997 and 1999. We calculated rate ratios (RRs) and 95% confidence intervals (CIs) for prostate cancer incidence associated with NSAID use, adjusting for age and potential 
prostate cancer risk factors. RESULTS: During follow-up from 1992-1993 through August 31, 2001, 4853 cases of incident prostate cancer were identified. Neither current 
aspirin use nor current use of NSAIDs (aspirin and other NSAIDs combined) was associated with prostate cancer risk, even at the highest usage level (60 or more pills per 
month). However, long-duration regular use (30 or more pills per month for 5 or more years) of NSAIDs was associated with reduced risk of prostate cancer (RR = 0.82, 95% CI 
= 0.71 to 0.94). Long-duration regular use of aspirin was also associated with reduced risk of prostate cancer (RR = 0.85, 95% CI = 0.73 to 0.99). The absolute rate of 
prostate cancer (standardized to the age distribution of study participants using 5-year age categories) was 1013 per 100,000 person-years among men who had never reported 
NSAID use, and 847 per 100,000 person-years among long duration regular NSAID users. CONCLUSIONS: These results support the hypothesis that long duration regular NSAID use 
is associated with modestly reduced risk of prostate cancer.

Drugs: [aspirin/ nonaspirin NSAIDs]
```

This abstract is not relevant since it discusses cancer risks and it does not discuss a treatment of cancer. Note the drug is not used as a treatment to avoid cancer reoccurrence. If the drug had been used to present cancer relapse, then the abstract would have been relevant for our study.

### Bonus Exercise

We are providing a csv file with 100 abstracts that are annotated whether they are relevant or not for our study. In the file, a relevant document is marked `include` and a irrelevant document is marked `exclude`. You are free to use any machine learning technique to build a binary classifier that given the PubMedID, the title and the abstract, predicts whether the paper is relevant or not. Since the dataset is rather small, we encourage you to use 5-fold cross validation to evaluate your models. 


## Acknowledgements:
- [IBM Research](https://researcher.watson.ibm.com/researcher/view.php?person=us-ioana)
- [Cures Within Reach for Cancer](https://www.cwr4c.org/)
