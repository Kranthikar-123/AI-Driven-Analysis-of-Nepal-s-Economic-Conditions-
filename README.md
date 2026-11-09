# AI-Driven-Analysis-of-Nepal-s-Economic-Conditions-

Using AI to Analyze the Economic State of Nepal, with the Use of Large Language Models, Extraction of Structured Data, and Retrieval-Augmented Generation

Project Overview

This study provides a methodology for developing a machine learning-based analytical platform that examines the economic and financial health of Nepal based on the IMF Country Report No. 23/158, issued in May 2023. The main objective of this study is to turn the unorganized data provided in the IMF report into actionable, organized, and understandable information via the use of NLP, LLM, data mining, and visual display methods.

The approach combines document processing, automated summarizing of documents, economic theme-based analysis, automated extraction of indicators from structured sources, qualitative assessment of risks, and Retrieval-Augmented Generation (RAG) into a single analytical process. Google Gemini Flash models are used to perform the language-based processing and analytical functions, whereas Python-based data science libraries assist with document preparation, numerical analysis, semantic retrieval, and visualizations.

This project utilized Google Colab to demonstrate the potential of modern AI methods for analyzing complicated macro-economic and financial documents.

Project Aim and Objectives

The main objective of the present study is to construct a system based on artificial intelligence (AI) that will be able to extract, organize, analyze, and present economic data from an IMF country report.

The process will extract all pertinent data from the source PDF, create an executive summary, create summaries for each section of the report, and examine the seven predetermined economic/financial topics. The process will also determine the most important macro-economic/banking indicators, evaluate the strengths/weaknesses of Nepal's economy, and develop a document-based question-and-answer platform using semantic retrieval.

The aim of this study is to create a visualization system that allows for analysis of the performance of various Gemini Flash models. Specifically, we will look at how well these models extract data, how compliant their outputs are with the rules, and how quickly they process the data.

Methodology and Implementation

The analytical process starts by extracting PDF text with the help of the PyPDF library. The extracted text is then cleaned up so that all unnecessary formats, headers, footers and other parts of the document are removed. The clean text is then broken down into 232 overlapping sections (or chunks) of text. Each section has a token length of about 400 and an overlapping token length of 50.

Using the Automated Summarization process, the document chunks are processed in 29 separate groups (batches) using Gemini 3.6 Flash. After processing all of the document chunks, the resulting summaries will then be combined through several processes to create an overall summary of the economic situation in Nepal.

Thematic analyses are conducted on 7 topics: Inflation & Prices; Interest Rates & Credit; Housing & Real Estate; Banking Capital & Liquidity; Sovereign Debt; Labor Market Dynamics; and Systemic Financial Risk. For each of these themes, a review is made to determine what significant economic changes have occurred (or are occurring), which indicators support those changes, how those changes compare with past trends, whether there exist vulnerabilities that could lead to financial instability, and what the potential impact of those changes might be.

Structured information extraction is used to pull predetermined macroeconomic and banking data out into JSON format. Data pulled out includes GDP growth estimates, core inflation, central bank interest rates, non-performing loans, unemployment rate and Tier 1 capital ratios. If the extracted data does not provide enough support for a specific number to be assigned to a field, then the field remains null instead of assigning a number that has no basis.

In addition, the project will use qualitative analysis to determine what aspects of Nepal's economy make it strong or weak. The resulting information is then organized into structured reports with accompanying data and economic results.

Retrieval-Augmented Generation

A Retrieval-Augmented Generation framework was developed to facilitate document-based question-answering. Sentence Transformers generated semantic embeddings for each of the document chunks based on the all-MiniLM-L6-v2 model. These embeddings were then indexed with FAISS, which allowed for the retrieval of matching passages via similarity search.

The system finds the passage that has been requested by the user, then generates an answer using Gemini 3.6 Flash from the information contained within that found passage. The system retains the original page number of the retrieved passage so that users may verify the accuracy of the information against the original IMF report.

This evaluation shows how the quality of retrieval and the selection of the most appropriate context affects the accuracy of responses. More specifically, retrieving only the relevant portion of the source material helped to identify the non-performing loan ratio reported in January 2023. This evidence illustrates the necessity of verifying and generating from sources as part of evaluating financial information.

Data Visualisation and Dashboard

An analytical visual dashboard has been created using pandas, matplotlib and seaborn so that the extracted economic data can be presented. The dashboard includes a combination of key performance indicators (KPIs) and graphs representing the current state of Nepal's economy and finances.

Visualizations will analyze trends in GDP growth and inflation, developments in public debt, analysis coverage of thematic issues and selected banking sector indicators. Pandas is used to apply data transformation techniques to convert wide-format data into long-format data structures to make the information available for visualization.

The dashboard presents a single display of the chosen economic measures, and provides assistance for interpreting previous events and expected future economic circumstances as described in the International Monetary Fund (IMF) report.

Comparative Model Evaluation

A comparative study has been performed with three different versions of the Gemini software: Gemini 3.5 Flash, Gemini 3.6 Flash, and Gemini 3.8 Flash. All three versions were assessed using the same structured extraction task based upon seven pre-defined economic/banking indicators.

The evaluation is based upon how well the model generates valid JSON output; the model's ability to produce accurate semantics; and the model's speed in generating responses. All three models had 100% accuracy in the seven fields evaluated after normalizing the semantics of numbers and percentages. While all three models were able to generate valid JSON output with 100% semantic accuracy, there was a large difference in how fast each model generated its response. Gemini 3.5 Flash had the fastest response time of 16.16 seconds. Next fastest was Gemini 3.6 Flash with a response time of 31.41 seconds. Lastly, Gemini 3.8 Flash took 357.60 seconds to generate a response.

The results of this experimental evaluation indicate that Gemini 3.5 Flash was both the fastest in terms of processing time and the most accurate in terms of semantic evaluation. However, the findings from this study are only valid for the conditions under which it was performed and do not provide an indication of the performance of each model on other tasks.

Technologies and Tools

The application was developed in Python in a Google Colab environment. The PDF content was extracted with PyPDF, and Pandas and NumPy provided support for preparing and processing data. Matplotlib and Seaborn created the visualizations that would assist in analysis.

The Gemini Flash models developed by Google are the foundation of LLM capabilities for summarization, thematic analysis and structured information extraction. The Sentence Transformers provided the capability to generate semantic embeddings, and the vector indexing and similarity-based retrieval functionality was provided by FAISS. Structured analytical outputs and intermediate results are stored in either JSON or CSV format.

Project Outcomes and Limitations

The result of this implementation shows how the system can automatically process a large IMF economic report by using automated document processing, as well as AI based analytical techniques. This process resulted in 29 summarizations, 7 thematic analysis, structured economic indicators, qualitative findings, a semantic retrieval system, and a consolidated economic dashboard.

Although some results have been achieved, there are still several limitations. Indicators that were not available within the collected data were coded as "missing" (or "null"). The performance of RAG depended on both the ability to retrieve relevant passages and select appropriate context. Finally, while the comparative model evaluation was based on a small sample of seven indicators, we would recommend further testing using a larger sample size.

Future enhancements may involve expanding the evaluation dataset, performing multiple model benchmarks, improving retrieval methods, and adding additional automated factual validation processes.

Source Document

International Monetary Fund (2023). Nepal: Staff Report for the 2023 Article IV Consultation, First and Second Reviews under the Extended Credit Facility Arrangement. IMF Country Report No. 23/158. Washington, DC: International Monetary Fund.

Author

This project was developed as an academic project.

Licence

This repository was created as an educational resource and an academic tool. The source code is offered under the MIT License. Please refer to the LICENSE file that accompanies this repository for the specific conditions of its use.
