# TEXT-SUMMARIZATION-TOOL

*COMPANY* : CODTECH IT SOLUTION

*NAME* : ELAINE JOSE

*INTERN ID* : CT04DN1322

*DOMAIN* : ARTIFICAL INTELLIGENCE

*DURATION* : 4 WEEKS

*MENTOR* : NEELA SANTOSH


The Natural Language Processing (NLP) Text Summarization project is a Python utility that automatically generates reduced summaries from huge text documents. With the contemporary era of living in the virtual world, processing and interpreting large texts is an imperative. This project aims to address the increasing demand for immediate consumption of content by providing an answer that extracts only the most important sentences from a document, giving an understandable summary and capturing the essence of the original content.

This type of summarization is extractive, in the sense that it selects and states primary sentences from the original text rather than generating new ones. The model merely reads a file, divides the material into sentences, computes similarities among sentences, and then uses PageRank algorithm to identify the most significant sentences.

The project applies a variety of fundamental Python libraries in order to accomplish its job:

NLTK (Natural Language Toolkit): To remove stopwords and perform basic pre-processing of text.

NumPy: For numerical computations, especially creating matrices of similarity.

NetworkX: To build a graph based on the sentence similarity matrix and to rank sentences based on the PageRank algorithm.

The algorithm then reads the text file in UTF-8 format to accommodate special characters. Stopwords (e.g., "is", "the", "in") are removed from each sentence as they do not carry meaning. A cosine similarity score is calculated for each sentence with each of the other sentences, creating a similarity matrix. It is used in an effort to create a graph where each sentence is a node and the nodes' edges are weighted using their similarity scores.

Once the graph has been built, PageRank, a graph-based ranking algorithm developed at Google, is applied. Each sentence is assigned a ranking score based on its connectivity to other high-scoring sentences. More highly scored sentences are believed to be more central and significant to the text.

From the ordered list, the N top sentences are selected and arranged in a format that can be easily read by humans. This is helpful for users to easily grasp the summary of lengthy articles, reports, or essays.

The code is modular and scalable. It accepts plain text (.txt) files and can be simply made to accept .docx files using the python-docx library. The number of sentences in the summary, or top_n, is also configurable, which makes the tool flexible enough for a wide range of applications such as academic research, journalism, and data analysis.

How it Works:
Input File: The user provides a .txt file.

Reading the File: The file is read line by line and taken as individual sentences.

Tokenization & Preprocessing: The sentences are cleaned, lowercased, and tokenized.

Similarity Matrix: Pairwise sentence similarity is calculated with cosine distance.

Graph Generation: The graph is created from the matrix using NetworkX.

Ranking Sentences: PageRank is used to rank every sentence.

Summary Generation: The best-ranked sentences are merged and presented as the summary.

The algorithm then loads the text file with UTF-8 encoding to handle special characters. The sentences are tokenized and stopwords (like "is", "the", "in") are excluded because they add little meaning. For every sentence, a cosine similarity measure is computed against each other sentence to create a similarity matrix. This matrix is used to construct a graph where each sentence is a node and the edge between nodes is based on their similarity scores.

Once the graph is built, PageRank, a ranking algorithm, is employed. The algorithm determines a ranking score for each sentence based on the quality of connection it has with other high-scoring sentences. The higher-scoring sentences are most central and connected to the text.

Out of the ranked list, the top N sentences are selected and output in a readable human format. This makes it easy for users to quickly comprehend the material of long articles, reports, or essays.

The code is modular and scalable. It accommodates plain text documents (.txt) and may be extended to accommodate .docx documents via the python-docx library. The summary sentence count (top_n) may be customized, making the tool flexible for a wide range of applications such as academic research, journalism, and data analysis.

Applications:
News summarization

Summarization of notes for academic research

Business intelligence reports

Technical and legal documents executive summaries

Technologies Utilized:
Python 3.x

NLTK (for tokenization and stopword removal)

NumPy (for matrix operations)

NetworkX (for sentence ranking)

Optional: python-docx for Word document support

Advantages:
Reduces reading time

Gathers key information in quick time

Easy to extend and customize

Ideal for automation and batch processing of document



