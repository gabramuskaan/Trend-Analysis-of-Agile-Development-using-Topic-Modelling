Topic-Modelling-using-Machine-Learning-LDA
Our project, "Trend Analysis of Agile Development using Topic Modeling," employs machine learning and Latent Dirichlet Allocation (LDA) to analyze trends in agile methodologies. By collecting and preprocessing data, extracting information with Pandas, applying LDA-based topic modeling, and optimizing coherence scores, we provide valuable insights for software engineering teams, enabling them to make data-driven decisions and drive continuous improvement in their agile development practices. Our project contributes to the software industry by fostering evidence-based decision-making and facilitating the adoption of best practices in agile development, ultimately leading to improved project outcomes and customer satisfaction.

(I)
TABLE OF CONTENTS

Chapter No.              Topics                                                                                                            

Chapter-1                Introduction 	                   
1.1                            General Introduction                                                                              
1.2                            Problem Statement                                                                             
1.3                            Significance/Novelty of the problem                                                  
1.4                            Empirical Study                                                                                       
1.5                            Brief Description of the Solution Approach                                           
1.6                            Comparison of existing approaches to the problem framed                   

Chapter-2                Literature Survey	
2.1                            Summary of papers studied                                                                   
2.2                            Integrated summary of the literature studied                                           

Chapter-3               Requirement Analysis and Solution Approach
3.1                            Overall description of the project                                                     
3.2                            Requirement Analysis                                                                           
3.3                            Solution Approach                                                                              

Chapter-4                Modeling and Implementation Details
4.1                            Design Diagrams
4.1.1                         Use Case diagrams                                                                                
4.1.2                         Flow Diagram                                                                                     
4.1.3                         Sequence Diagram/Activity diagrams                                                  
4.2                            Implementation details                                                             
4.3                            Risk Analysis and Mitigation                                                       

Chapter-5               Testing (Focus on Quality of Robustness and Testing)
5.1                            Testing Plan                                                                                                             
5.2                            Component decomposition and type of testing required                       
5.3                            List all test cases in prescribed format                                          
5.4                            Error and Exception Handling                                               
5.5                            Limitations of the solution                                                                  

Chapter-6                Findings, Conclusion, and Future Work
6.1                             Findings                                                                                             
6.2                             Conclusion                                                                                           
6.3                             Future Work  
                                Reference

         


SUMMARY

The project "Topic Modeling using Latent Dirichlet Allocation" is a machine learning project that uses the Latent Dirichlet Allocation (LDA) algorithm to identify topics within a set of documents. LDA is a probabilistic model that assumes each document is a mixture of topics and each topic is a mixture of words. The goal of LDA is to infer the topic distribution of each document and the word distribution of each topic. The project involves several steps, including data preprocessing, running the LDA algorithm, and evaluating the results. In data preprocessing, the raw text data is cleaned and transformed into a format suitable for LDA analysis. LDA is then run on the document-term matrix to identify the topics present in the data. Finally, the results are evaluated using metrics such as coherence and topic diversity. The project has many applications, such as identifying topics in social media data, analyzing customer reviews, and identifying trends in research papers. LDA has proven to be a powerful tool for topic modeling and has been widely used in various fields.


Chapter-1:   Introduction	                   
1.1   General Introduction
The growth of digital data has led to an explosion of unstructured text data, which has created a need for automated techniques to analyze and extract meaningful information from these vast amounts of data. Topic modeling using Latent Dirichlet Allocation (LDA) is a technique that helps us to extract meaningful information from large collections of unstructured text data, which can be used in various applications such as marketing, social media analysis, e-commerce, and healthcare. By using LDA, it is possible to identify trends, sentiments, preferences, and patterns, which can help in making informed decisions and developing effective strategies. The technique has been used in various real-life scenarios such as content analysis, analyzing news articles in finance, information retrieval, recommendation systems, etc. 

1.2   Problem Statement
The problem statement of the project "Topic Modeling using Latent Dirichlet Allocation" is to identify latent topics within a set of documents, which can be a time-consuming and challenging task for humans to perform manually. The project aims to address this problem by using machine learning techniques to automatically identify and extract the underlying topics within a large corpus of documents, thereby saving time and increasing accuracy. 

1.3   Significance/Novelty of the problem
The problem addressed in the project "Topic Modeling using Latent Dirichlet Allocation" is significant because it addresses the challenge of identifying latent topics within a large corpus of unstructured text data. Topic modeling is a fundamental task in natural language processing and has numerous applications, such as understanding customer feedback, tracking trends in social media, and identifying key themes in scientific research. The use of LDA for topic modeling is particularly significant because it is a powerful and flexible algorithm that can effectively identify latent topics in large datasets. This makes it a valuable tool for researchers and practitioners in many fields who need to analyze and make sense of large volumes of unstructured text data. Overall, the project's significance lies in its ability to demonstrate the power and versatility of LDA for topic modeling, and to provide a clear and accessible example of how advanced machine learning techniques can be applied to real-world problems with significant impact.

1.4   Empirical Study (Field Survey/Existing Tool/Survey/Experimental Study)
With the explosion of digital data in recent years, organizations are facing a daunting challenge of managing and making sense of massive amounts of unstructured text data. Topic modeling, as showcased in this project, offers a powerful solution to this challenge by automatically identifying the key themes and topics present within a large corpus of text data. One of the most important applications of topic modeling is in the field of market research and customer analytics. By analyzing customer reviews, social media data, and other sources of unstructured text data, organizations can gain insights into customer preferences, opinions, and sentiments. This, in turn, can help businesses make data-driven decisions about product development, marketing strategies, and customer engagement. In addition, topic modeling can be used in scientific research to identify emerging trends and topics in a given field. By analyzing large volumes of research papers and other academic literature, researchers can identify key topics and areas of focus, helping to drive innovation and discovery. Overall, the project "Topic Modeling using Latent Dirichlet Allocation" highlights the importance of topic modeling in today's data-driven world. As the volume of unstructured text data continues to grow, topic modeling offers a powerful solution for making sense of this data and extracting valuable insights.

1.5   Brief Description of the Solution Approach
Latent Dirichlet Allocation (LDA) is a widely used technique in topic modeling. The basic idea behind LDA is that each document in a corpus is represented as a mixture of topics, and each topic is a probability distribution over words. The algorithm assumes that each word in a document is generated by one of the topics in the document's mixture, and each topic generates words with a certain probability distribution. The goal of LDA is to infer the topic mixture for each document and the word distribution for each topic that best explains the observed corpus.

The LDA algorithm works as follows:
●	Initialize the number of topics and the topic-word distribution for each topic.
●	For each document in the corpus, assign each word in the document to a topic randomly.
●	For each word in each document, compute the probability of the word belonging to each topic, based on the current topic-word distribution and the current assignment of the other words in the document.
●	Reassign each word to a new topic based on the computed probabilities.
●	Repeat steps 3 and 4 until convergence, i.e., until the topic mixture for each document and the word distribution for each topic stabilize.
●	Once the algorithm converges, the resulting topic mixture for each document and the word distribution for each topic can be used for various tasks such as document classification, topic summarization, and information retrieval.

Overall, LDA is a powerful technique that allows us to uncover latent topics in a corpus and provides a way to represent documents in a low-dimensional topic space.


1.6  Comparison of existing approaches to the problem framed
There are several existing approaches to topic modeling, and LDA is just one of them. Here are some comparisons of LDA with other approaches:
●	LSA (Latent Semantic Analysis): LSA is an earlier technique for topic modeling that uses Singular Value Decomposition (SVD) to identify the latent topics in a corpus. However, LSA suffers from the problem of not being able to model words that do not occur in the training data. LDA, on the other hand, can generate new words based on the learned word distributions.
●	NMF (Non-negative Matrix Factorization): NMF is another technique for topic modeling that has been shown to work well in some applications. NMF is faster than LDA, but it does not handle the sparsity of the term-document matrix well. LDA can handle this sparsity by modeling the topic-word and document-topic distributions as Dirichlet distributions.
●	PLSA (Probabilistic Latent Semantic Analysis): PLSA is a precursor to LDA that models the joint distribution of words and documents directly. However, PLSA suffers from overfitting, especially for large vocabularies. LDA, on the other hand, regularizes the word distributions with a Dirichlet prior, which prevents overfitting.
In summary, LDA is a widely used technique for topic modeling that has been shown to work well in many applications. While other techniques such as LSA, NMF, and PLSA have their own strengths and weaknesses, LDA is often the default choice for topic modeling due to its flexibility, scalability, and ease of use.


Chapter-2:   Literature Survey	
2.1   Summary of papers studied

1. In the research paper titled "Topic Modeling for Software Engineering: An Experience Report" the authors propose using LDA for software engineering applications such as bug triage and software traceability. The paper presents a case study of using LDA for bug triage in a large software project. One of the strengths of this paper is its practical focus on applying LDA to a real-world software engineering problem.
Link: https://link.springer.com/chapter/10.1007/978-3-642-13657-3_43

2. The research paper titled "Research Patterns and Trends in Software Effort Estimation" uses LDA to analyze research trends in software effort estimation. The authors apply LDA to a corpus of research papers and identify key topics and trends in the field of software effort estimation. Its use of LDA gains insights into a specific research field. 
Link: https://www.researchgate.net/publication/317507973_Research_Patterns_and_Trends_in_Software_Effort_Estimation

3. The research paper titled "Topic modeling for dynamic feature selection in text categorization" proposes using LDA for dynamic feature selection in text categorization. The authors propose a novel algorithm that uses LDA to select features based on their relevance to the topic. 
Link: https://www.sciencedirect.com/science/article/abs/pii/S092523120800372X

In summary, all three papers demonstrate the usefulness of LDA for various applications, but they all have gaps in terms of the evaluation of the LDA model's performance. 


2.2    Integrated summary of the literature studied
The research papers focus on the use of topic modeling techniques in software engineering and related fields. The papers demonstrate the utility of topic modeling algorithms such as LDA in identifying and analyzing key topics within software engineering datasets, including effort estimation research and text classification tasks. Additionally, the papers highlight the versatility of topic modeling, showcasing its application in various domains and contexts. These studies illustrate the critical importance of topic modeling techniques in enabling researchers and practitioners to extract insights and make informed decisions from large and complex datasets.


Chapter-3:  Requirement Analysis and Solution Approach
3.1  Overall description of the project 

●	Data Collection and Preprocessing: The first step in our topic project is to collect the data and preprocess it. We first collected about 1000 documents using the Zotero application and then cleaned it, also removed the duplicates.  This involves cleaning the text data by removing stopwords, punctuations, and other noise, and transforming the data into a format that can be used by the LDA algorithm.
●	Exploratory Data Analysis (EDA): Once the data is preprocessed, EDA is performed to gain insights into the data. EDA involves techniques such as frequency analysis, word cloud generation, and topic visualization.
●	Model Building and Training: The next step is to build an LDA model and train it on the preprocessed data. The LDA model learns the topic distributions for each document and the word distributions for each topic. The number of topics needs to be specified beforehand or can be determined using techniques such as grid search or cross-validation.
●	Model Evaluation: After training the LDA model, it is evaluated using various metrics such as coherence score. These metrics help to assess the quality of the topics generated by the LDA model.
●	Topic Interpretation and Visualization: Once the LDA model is evaluated, the topics generated by the model are interpreted and visualized with the help of bar graph and time series graph.
●	Optimization: We have optimized the hyperparameters and generated a new coherence score.
●	Applications: Finally, the topics generated by the LDA model can be used for various applications such as document classification, sentiment analysis, recommendation systems, and information retrieval.

Overall, our project on using LDA in topic modeling involves collecting and preprocessing data, building and training an LDA model, evaluating the model, interpreting, visualizing the topics generated by the model and optimizing the day, hence using the topics for various applications.


3.2   Requirement Analysis (Functional/Non-Functional/Logical Database requirements)

1.	Functional Requirements:
Functional requirements refer to the features and functionalities that the topic modeling system must provide. Some functional requirements for LDA topic modeling include:
●	Ability to preprocess and transform text data into a format that can be used by LDA.
●	Ability to train an LDA model on the preprocessed data.
●	Ability to specify the number of topics for the LDA model.
●	Ability to evaluate the LDA model using coherence score, perplexity, and topic diversity.
●	Ability to interpret and visualize the topics generated by the LDA model.
●	Ability to use the topics generated by the LDA model for various applications such as document classification, sentiment analysis, and recommendation systems.

2.	Non-Functional Requirements:
Non-functional requirements refer to the performance, usability, security, and other non-functional aspects of the topic modeling system. Some non-functional requirements for LDA topic modeling include:
●	Performance: The system must be able to train the LDA model and generate topics within a reasonable time frame.
●	Usability: The system must be easy to use and provide clear instructions for each step in the process.
●	Security: The system must be secure and protect sensitive data.
●	Scalability: The system must be able to handle large volumes of data and scale up as needed.
●	Compatibility: The system must be compatible with different operating systems, programming languages, and hardware platforms.

3.	Logical Database Requirements:
Logical database requirements refer to the data structure and storage requirements for the topic modeling system. Some logical database requirements for LDA topic modeling include:
●	Data Import and Processing: The first logical database requirement would be to import the data from the CSV file into the pandas data frame and preprocess the data for topic modeling. This might involve removing stop words, stemming or lemmatizing the text, and converting the text to a bag-of-words.
●	Topic Interpretation and Visualization: The second logical database requirement would be to interpret and visualize the extracted topics. This might involve identifying the most representative terms for each topic, visualizing the relationship between topics using techniques such as bar graph, time series graph, and identifying the most relevant documents or passages associated with each topic.
●	Storage and Retrieval: Finally, the logical database requirement would be to store the preprocessed data, the trained LDA model, and the output results in a structured format for future retrieval and analysis. It is also optimized and hence generated a new coherence score. This might involve storing the data in a database management system such as SQLite or MongoDB, or in a cloud-based storage service such as Google Cloud Storage.


3.3   Solution Approach (algorithms or hardware used)

The solution approach for the project "Topic Modeling using Latent Dirichlet Allocation" involves several steps, including data preprocessing, creating a document-term matrix, running the LDA algorithm, and evaluating the results. The following is an overview of the solution approach:
1. The raw text data is cleaned and transformed into a format suitable for analysis by the LDA algorithm. This may involve tasks such as tokenization, stemming, and stopword removal.
2. The preprocessed data is represented as a document-term matrix, which captures the frequency of each term in each document. This matrix serves as the input to the LDA algorithm.
3. The LDA algorithm is run on the document-term matrix to identify the topics present in the data. The algorithm assumes that each document is a mixture of topics, and each topic is a mixture of words. The goal is to infer the topic distribution of each document and the word distribution of each topic.
4. The results of the LDA algorithm are evaluated using various metrics, such as coherence and topic diversity. These metrics help assess the quality and interpretability of the topics identified by the algorithm.
5. The topics identified by the LDA algorithm can be visualized using various techniques, such as word clouds, topic networks, and topic proportions over time. These visualizations help users understand and interpret the results.
6. A new coherence score would be generated by optimizing the hyper parameters.

Overall, the solution approach for the "Topic Modeling using Latent Dirichlet Allocation" project involves a rigorous and systematic process for identifying latent topics within a corpus of documents. The approach relies on a combination of data preprocessing, statistical modeling, and visualization techniques to generate insights and drive decision-making.


Chapter-4:   Modeling and Implementation Details
4.1   Design Diagrams
      4.1.1  Use Case diagrams  
      ![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/eb7de49d-996d-44d9-983a-90a5e09bf5dc)

 4.1.2    Flow Diagram
 ![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/31be9cf5-0547-4c58-a7a0-145d4712f1fa)      
 
 4.1.3   Sequence Diagram/Activity diagrams
 ![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/f89aca01-cc37-44d4-99d4-7566e8a12cc0)


4.2   Implementation details 

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/095f54e1-2f03-444a-a4fd-301218c680c9)
 

The following are some of the implementation details for this project:
1. Data preprocessing: Before applying the LDA algorithm, the raw text data must be preprocessed to remove any unwanted characters, convert text to lowercase, and apply other text cleaning techniques. Additionally, the data is tokenized and transformed into a numerical format, such as a document-term matrix.
2. LDA model training: The LDA algorithm is applied to the preprocessed data to infer the topic distributions of each document and the word distributions of each topic. The model parameters, such as the number of topics and the alpha and beta priors, can be tuned to optimize the model's performance.
3. Evaluation metrics: The quality of the topics identified by the LDA algorithm is evaluated using various metrics, such as coherence, topic diversity, and topic uniqueness. These metrics help to assess the effectiveness of the LDA model and identify areas for improvement.
4. Visualization: The results of the LDA model are visualized using various techniques, such as word clouds, topic clusters, and topic proportions. Visualization is an important component of the project as it enables users to quickly and easily understand the insights gained from the data.

These processes work together to enable the effective identification and analysis of latent topics within large volumes of textual data.


Features built, language used:
We built a topic modeling system using LDA that can discover hidden topics in a collection of text documents. Python programming language was used to implement the system. The system also includes features such as data preprocessing, topic visualization, and topic evaluation metrics.

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/b6f042ac-1fe2-48ef-919b-fef29bffd1c8)
All the necessary packages were imported.

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/b8abacb7-8ffa-453b-8941-e713a6ffd064)
Data preprocessing was done which included removal of punctuations, numerical values, stop words and Stemming using the Snowball Stemmer algorithm.

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/44fe340e-287d-44c4-b964-6989d79399e5)
The preprocessed data was converted into a bag of word representation to proceed with the learning process.

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/44ceac02-bb3b-4491-9018-7b292da5bd73)
Initially we set the number of topics as 8 and the values of the hyperparameters Alpha and Beta were set to default.
 
![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/c258b3a3-1104-454b-8ce7-9926c9591fe8)
This visualization shows the Mean Probability Distribution of each topic across all the documents.

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/c5bccdb1-4b0a-4607-92e2-d5caa89d86d9)
This visualization shows a time series of the Topic Distribution over the period of 1990 - 2020.

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/1f08b5ce-0638-42ec-8187-6febef0d91fd)
The coherence score of the trained model was calculated.

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/03161ba3-5b94-4f3b-9511-775d61201bcb)
Lastly, we attempted to optimize our coherence score.

4.3   Risk Analysis and Mitigation

Like any other data analysis technique, topic modeling using LDA comes with its own set of risks and challenges. Here are some of the major risks that should be considered when using LDA for topic modeling and their corresponding mitigation strategies:
●	Overfitting: Overfitting is a common risk when using machine learning algorithms, including LDA. Overfitting occurs when the model is trained too closely on the training data and becomes too specialized to that particular dataset, resulting in poor generalization on new data. To mitigate this risk, it is important to perform cross-validation and use regularization techniques such as adding a penalty term to the likelihood function to prevent overfitting.
●	Selection of the Number of Topics: Choosing the appropriate number of topics is a critical decision in LDA topic modeling. Selecting too few or too many topics can result in low-quality topics or topics that overlap, respectively. To mitigate this risk, it is recommended to use techniques such as grid search and cross-validation to determine the optimal number of topics.
●	Quality of Data: The quality of the data can have a significant impact on the quality of the topics generated by LDA. If the data is noisy, has missing values, or is biased, it can result in poor quality topics. To mitigate this risk, it is important to perform data cleaning and normalization before applying LDA. This can include removing stopwords, stemming, and filtering out infrequent terms.
●	Interpretation of Topics: The interpretation of the topics generated by LDA can be subjective and may require domain expertise. It is possible for the topics to be difficult to interpret or for multiple interpretations to be valid. To mitigate this risk, it is recommended to involve domain experts in the interpretation process and to perform qualitative evaluation of the topics.
●	Scalability: LDA can become computationally expensive for large datasets, which can result in long training times and memory constraints. To mitigate this risk, it is recommended to use distributed computing platforms or to implement LDA using a parallel computing approach.
●	Privacy and Security: Sensitive information can be present in the data, which can pose risks to privacy and security. To mitigate this risk, it is important to ensure that the data is properly anonymized and that access to the data and the model is restricted.


Chapter-5:   Testing
5.1  Testing Plan

For the testing part we ran some tests for tuning the hyper-parameters of the LDA model in such a way so that our coherence score would be optimal. We iterated on every value of the Alpha and Beta parameter while also changing the number of topics to get the best value for our model that would optimize our coherence score. 

5.2  Component decomposition and type of testing required

The testing for the optimality of the coherence score was done in a brute-force manner in order to cover every possible value that can result in a better value for the coherence score.

5.3    List all test cases in prescribed format

There was only one test for the optimality of the coherence score in which we iterated over every value of the number of topics, Alpha-value and Beta-value in a nested loop.

![image](https://github.com/gabramuskaan/Trend-Analysis-of-Agile-Development-using-Topic-Modelling/assets/124431862/e91ed1f4-c945-4510-979d-e16212ba4271)

These are all the values of the number of topics, Alpha, Beta and the coherence score that were obtained by trying every permutation possible to get the maximum coherence score.


5.3    Error and Exception Handling   

The errors were:
1. There was an error message saying that we cannot use the get_feature_names() method from the CountVectorizer class. This method has been deprecated in version 1.0 and will be removed in version 1.2. So, to fix this we used the get_feature_names_out() method, which was introduced in version 1.0 as a replacement for get_feature_names().
2. While plotting the time series graph which shows the trend we encountered an error "TypeError: 'numpy.float64' object cannot be interpreted as an integer", which was fixed by type casting the float value as an integer using "int()".
3. We encountered an error where the "doc2bow()" method expects an array of tokens as input but we were providing strings. So to fix this we applied the "doc2bow()" method on each inner string. 

The exception was:
1. While creating a bag of words matrix using the Count Vectorizer we encountered an exception in which some of the places in the 'Abstract Note' column of the database were missing. So in order to handle that we replaced any missing values in that column with an empty string using the 'fillna' method.


5.5    Limitations of the solution

 Some of the limitations of the LDA model are:
●	Interpretability: Although the topics generated by the LDA model are typically human-readable, they may not always be interpretable. This is especially true when the number of topics is high or when the topics are very similar to each other.
●	Scalability: LDA can become computationally expensive as the number of documents and the number of topics increases. This can make it difficult to use LDA on large datasets.
●	Sparsity: The LDA model assumes that documents are generated from a mixture of topics, but in reality, documents may only contain a few topics. This can result in sparse topic-document matrices, which can affect the quality of the topics generated by the model.
●	Sensitivity to parameters: The performance of LDA can be highly dependent on the choice of hyperparameters, such as the number of topics and the alpha and beta parameters. It can be difficult to choose the optimal set of hyperparameters for a given dataset.
●	Lack of temporal information: The LDA model assumes that documents are generated independently of each other, which means that it cannot capture the temporal dynamics of the data. This can be a significant limitation when working with time-series data.


Chapter-6:  Findings, Conclusion, and Future Work
6.1   Findings

●	LDA can be used to identify the most important topics present in a corpus of text. These topics can provide insights into the underlying themes and patterns present in the text and are known as key topics.
●	Topic modeling using LDA can also be used to visualize the relationships between different topics. This can be particularly useful for identifying topics that are related or that overlap in meaning.
●	LDA can be used to analyze changes in topic prevalence over time. This can be particularly useful for identifying emerging topics or tracking changes in public opinion or interest.
●	LDA can be used to identify domain-specific terminology that is commonly used within a particular field or industry. This can be useful for identifying key concepts and terminology that may be unfamiliar to those outside the field.
●	Finally, a project on topic modeling using LDA may also involve evaluating the performance of the LDA model. This can be done by comparing the model's results to a gold standard dataset or by using quantitative metrics such as coherence or perplexity scores. This evaluation can provide insights into the strengths and limitations of the LDA model and can inform future improvements to the model.


6.2   Conclusion

At the end of our project we learned the basics of Unsupervised Machine Learning. We  explored different ML algorithms through which we got to know about the one we implemented i.e LDA (Latent Dirichlet Allocation). We were able to handle and manipulate large datasets using the inbuilt packages provided by Python. All this knowledge helped us to perform trend analysis on the domain of Requirements Engineering.


6.3    Future Work

There are several potential areas for future work on this some possible directions include:
●	We will explore additional models as LDA is a popular and effective topic modeling algorithm, there are many other models that could be used for trend analysis.
●	We will Fine tune the model as hyperparameter tuning can help to improve the performance of an LDA model. Future work could involve experimenting with different values for the alpha and beta hyperparameters and using cross-validation techniques to find the optimal values.
●	We will incorporate additional features as there may be other features in addition to the text data that could be used to improve trend analysis. For example, metadata such as author names, publication dates, and journal titles could provide valuable information for understanding trends in a particular field.
●	We will conduct comparative analysis as it may be interesting to compare the results of LDA trend analysis with other methods for identifying trends in the literature. For example, manual literature reviews or citation analysis could be used to evaluate the accuracy of the LDA model.
●	Finally, we will extend the analysis, while this project focused on trend analysis in a single field (Requirements Engineering), the methods could be applied to other fields as well. Future work could involve adapting the LDA model to other domains and exploring how trends differ across different fields.


References   

[1]	“An introduction to Bag of Words in NLP using python,” Great Learning Blog: Free Resources what Matters to shape your Career!, 11-Sep-2020. [Online]. Available: https://www.mygreatlearning.com/blog/bag-of-words/. 
[2]	D. M. Blei, A. Y. Ng, and M. I. Jordan, “Latent Dirichlet Allocation,” Jmlr.org, 2003. [Online]. Available: https://www.jmlr.org/papers/volume3/blei03a/blei03a.pdf. 
[3]	S. Kapadia, “Evaluate topic models: Latent Dirichlet allocation (LDA),” Towards Data Science, 19-Aug-2019. [Online]. Available: https://towardsdatascience.com/evaluate-topic-model-in-python-latent-dirichlet-allocation-lda-7d57484bb5d0. 
[4]	“pandas: Get the number of rows, columns, elements (size) of DataFrame,” Nkmk.me, 12-Jul-2019. [Online]. Available: https://note.nkmk.me/en/python-pandas-len-shape-size/. 
[5]	“Python,” GeeksforGeeks, 03-Jul-2018. [Online]. Available: https://www.geeksforgeeks.org/python-pandas-apply/. 
[6]	“Pandas,” PyPI. [Online]. Available: https://pypi.org/project/pandas/. 
[7]	“Visual paradigm online,” Visual-paradigm.com. [Online]. Available: https://online.visual-paradigm.com/share.jsp?id=323430313736382d33.


