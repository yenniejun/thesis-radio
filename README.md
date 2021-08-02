# Tuning In: COVID-19 Vaccine Discourse on Public Radio in South Africa and Nigeria

This is the Jupyter notebook that accompanies my Masters dissertation ([MSc in Social Data Science](https://www.ox.ac.uk/admissions/graduate/courses/msc-social-data-science?wssl=1) at the Oxford Internet Institute). 

This thesis is done in partnership with the UN Global Pulse (UNGP) and WHO. 
This project monitors and analyzes discourse on public radio stations from differnet countries across the African continent. 
Read more about the project [here](https://www.who.int/news/item/04-05-2021-who-and-un-global-pulse-are-building-a-social-listening-radio-tool-to-aid-the-covid-19-infodemic-response).

## Data
Radio transcriptions from South Africa and Nigeria

## Tools 
* `nltk` for text cleaning and processing
* `spaCy` for lemmatization
* `gensim` for training (Word2Vec) embeddings

## Abstract
The _infodemic_, as defined by the World Health Organization (WHO), is characterized by excessive amounts of information, including misinformation, rumors, and conspiracy theories. Overabundance of information is particularly harmful during public health crises, such as the current COVID-19 pandemic, due to increased difficulty of finding trustworthy sources and reliable guidance.
The circulation of rumors concerning the origin of the disease, alternative treatments, and vaccine side effects have led to distrust in public health organizations and mass vaccination efforts. 
Developing tools and methodologies for parsing large infodemic data sources can help decision makers understand conversations to shape the best policy choices.

While many existing tools monitor discourse from online forums and social media platforms, there are currently no scalable tools for monitoring discourses held on radio. Radio remains a major communication tool in many countries and has several benefits over social media, such as having higher coverage in developing nations and providing more context on conversations rather than being limited to short Tweets or Facebook posts. To ensure that no voices are left behind, it is imperative for public health officials to monitor discourses on radio.

This study aims to evaluate semantic shifts of discourse related to vaccine distribution and side effects during the COVID-19 pandemic on public radio streams from South Africa and Nigeria.
_Temporal word embeddings_ are used to determine the words that consistently describe vaccine discourse for each country over a period of eight weeks in 2021. 
To address the instability of word embedding models, over 800 models are trained by bootstrapping training documents.
Using the ensemble of bootstrapped models, the role of local and global real-world events in shaping vaccine discourse is evaluated.  
Finally, these results are operationalized by translating the above insights into a decision-making tool to empower public health officials for better understanding, combating, and monitoring the infodemic.