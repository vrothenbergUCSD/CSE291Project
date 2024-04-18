## CSE 291 Project : Sentiment Analysis and Automated Medical Summarization in Clinical Notes for Enhanced Patient Care

### Members 
- Vince Rothenberg A16534656
- Amogh Patankar A16580842
- Nicholas Chua A16584026
- Aashish Bhole A59016395
  
### Datasets
MIMIC-IV v2.2 is a large dataset containing comprehensive hospital wide electronic health records and ICU reports. In addition, we plan on using the MIMIC-IV-Note dataset, which contains de-identified free-text clinical notes. If time permits we will use a web scraped dataset of the subreddit AskDoc for medical Q&A. 
Research Problem: Understanding patient sentiment and efficiently summarizing clinical narratives are crucial for improving patient care and outcomes. However, the vast amount of unstructured text in clinical notes poses a challenge for healthcare providers in extracting meaningful insights promptly.

### Objective
To develop a comprehensive text mining system that performs sentiment analysis on clinical notes to gauge patient sentiment over time, and employs automated summarization algorithms to generate concise patient histories and summaries of hospital stays. This system aims to aid healthcare providers in making informed decisions quickly and understanding patient experiences and outcomes more effectively.
Related Works: In the medical AI domain, there is a lot of research with regards to NLP tasks on the MIMIC-III dataset, a precursor to the more robust MIMIC-IV dataset, as well as lesser research upon the MIMIC-IV dataset itself. We intend to dive deeper into the analyses derived from advanced NLP and text mining systems when run upon the MIMIC-IV database, in order to retrieve more complex insights. 

### Proposed Solution

**Sentiment Analysis:** Utilize NLP techniques to analyze sentiment in clinical narratives, tracking changes in patient sentiment throughout their hospital stay. This analysis will help identify patterns related to patient experience, treatment responses, and overall satisfaction.

**Automated Medical Summarization:** Develop extractive and generative summarization models to create succinct and informative summaries of patient records, enhancing the efficiency of reviewing patient histories and facilitating quicker decision-making processes.

**Unsupervised Information Extraction:** Implement unsupervised learning methods to extract key medical entities (diseases, symptoms, medications, procedures) from the clinical notes, enabling a structured representation of the unstructured text data.

### Methodology
Perform exploratory data analysis on MIMIC-IV clinical notes to understand the data structure, identify key variables, and guide the development of text mining models.

Apply advanced NLP techniques such as NER, sentiment analysis, and text summarization using the latest LLMs, adapting these models to the medical domain.

Fine tuning of models from HuggingFace, such as bert-base-uncased, BioBERT, ClinicalBERT, GPT-3, and T5, will be performed on MIMIC-IV's clinical notes for sentiment analysis and medical summarization. We will also consider more recent open source Ollama models like Mistral 7B.

### Evaluation Plan

Compare sentiment analysis results with patient outcomes (e.g. ICD diagnosis codes, discharge type, disease progression) to validate the correlation between patient sentiment and clinical results.

Assess the quality of generated summaries by their ability to capture critical information as evaluated by medical professionals. 

Benchmark the unsupervised information extraction performance against existing supervised methods to demonstrate efficacy and accuracy, precision, recall.

### Significance
This project will provide novel insights into patient experiences and streamline the review process of medical records, contributing to improved patient care and operational efficiency in healthcare settings. By leveraging the rich, de-identified clinical data in MIMIC-IV, the project also aims to advance the field of clinical NLP and support future research and applications in healthcare informatics.

### Workload Distribution

We plan for all members to distribute tasks evenly, namely data cleaning and preprocessing, running various NLP and ML models on the dataset, as well as writing the project report. Vince applied for access to the MIMIC dataset, downloaded the files, and will conduct preliminary data exploration as well as model construction. We will have more clarity as we begin to work on the project itself. 


### References

Johnson, Alistair, et al. "MIMIC-IV" (version 2.2). PhysioNet (2023), https://doi.org/10.13026/6mm1-ek67.

Johnson, Alistair, et al. "MIMIC-IV-Note: Deidentified free-text clinical notes" (version 2.2). PhysioNet (2023), https://doi.org/10.13026/1n74-ne17.

Fostiropoulos. "AskDoc." GitHub, repository, 2024, https://github.com/fostiropoulos/AskDoc.

Jiang, Albert Q., et al. "Mistral 7B." arXiv preprint arXiv:2310.06825 (2023).

Wang, G., Liu, X., Ying, Z. et al. Optimized glycemic control of type 2 diabetes with reinforcement learning: a proof-of-concept trial. Nat Med (2023). https://doi.org/10.1038/s41591-023-02552-9






