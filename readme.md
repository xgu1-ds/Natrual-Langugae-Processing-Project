Spring 2020 (#32961)

  * David Kurniadi

  * Rene Lizarraga

  * Xin Gu

# COVID-19 Open Research Dataset Challenge (CORD-19)

## Introduction
Corona Virus Disease 2019 (COVID-19) is a contagious respiratory illness caused by a novel coronavirus.  Although we are still learning about the origins of the virus, we know the first cases were reported after a cluster of severe pneumonia cases on New Year’s Eve 2019 in Wuhan, China. The virus has spread rapidly with the first confirmed case in the United States reported on January 20, 2020 (Holshue, 2019).  According to the World Health Organization (WHO, 2020), as of April 19, 2020, there are over 2.2 million confirmed cases worldwide and 152,707 deaths worldwide, with 695,353 and 32,427 of those being in the United States, respectively.  As infections and the death toll continue to rise worldwide, scientists and medical researchers race to both contain the spread of the virus and develop a vaccine. 
Artificial Intelligence (AI) can help medical researchers fight the virus by scouring tens of thousands of relevant research papers at an unprecedented pace (Etzioni, 2020).  In fact, Kaggle, an online community of data scientists and machine learning practitioners published an open competition (“COVID-19 Open Research Dataset Challenge (CORD-19)”) to analyze over 52,000 scholarly articles, including 41,000 with full-text, about COVID-19, SARS-CoV-2, and related coronaviruses.  The competition is an attempt to support the ongoing COVID-19 response efforts worldwide through the implementation of Natural Language Processing (NLP) to quickly mine the literature to answer key scientific questions (Kaggle, 2020).  There are 10 tasks as part of the challenge.  We have selected to focus on one the tasks; “What is known about transmission, incubation, and environmental stability?”  This task has 14 task questions to answer as listed below. 
1.	Range of incubation periods for the disease in humans (and how this varies across age and health status) and how long individuals are contagious, even after recovery.
2.	Prevalence of asymptomatic shedding and transmission (e.g., particularly children).
3.	Seasonality of transmission.
4.	Physical science of the coronavirus (e.g., charge distribution, adhesion to hydrophilic/phobic surfaces, environmental survival to inform decontamination efforts for affected areas and provide information about viral shedding).
5.	Persistence and stability on a multitude of substrates and sources (e.g., nasal discharge, sputum, urine, fecal matter, blood).
6.	Persistence of virus on surfaces of different materials (e,g., copper, stainless steel, plastic).
7.	Natural history of the virus and shedding of it from an infected person
8.	Implementation of diagnostics and products to improve clinical processes
9.	Disease models, including animal models for infection, disease and transmission
10.	Tools and studies to monitor phenotypic change and potential adaptation of the virus
11.	Immune response and immunity
12.	Effectiveness of movement control strategies to prevent secondary transmission in health care and community settings
13.	Effectiveness of personal protective equipment (PPE) and its usefulness to reduce risk of transmission in health care and community settings
14.	Role of the environment in transmission
Our contribution is to apply Natural Language Processing (NLP) techniques to the journal corpus to help scientists and researchers get quick answers to these questions about COVID-19 to expedite their goals. 
We compare 3 approaches to answer the task questions, evaluate the results, and assess the pros and cons of each approach.  The first approach applies Latent Dirichlet Allocation (LDA) to retrieve relevant medical articles, leaving it to the researcher to read the article in order to find the task answers within the article. The second approach applies Global Vectors of Work Representation (GloVe) and Cosine Similarity together to evaluate the corpus to retrieve relevant text that answers the questions.  The third approach combines the first two approaches; Latent Dirichlet Allocation (LDA) retrieves the relevant medical articles and then runs GloVe with Cosine Similarity on those articles to provide the text to answer the questions. 
We then evaluate the results by reading the retrieved article and text from each approach and evaluate if the question is answered.  

