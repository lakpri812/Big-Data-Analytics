# Big-Data-Analytics

Question 1 – Named Entity Recognition with Word Count
We implemented a Named Entity Recognition system using spaCy and PySpark to analyze the "Sherlock Holmes" book. Following steps were involved:

-- Loaded text from Databricks DBFS.
-- Installed and loaded spaCy with the en_core_web_md model.
-- Defined a function extract_named_entities() to extract entities of types: PERSON, ORG, GPE, LOC, NORP, PRODUCT, DATE, MONEY, FAC.
-- Processed text as RDD: Mapped lines to named entities and Flattened and reduced RDD to count frequencies.
-- Sorted and displayed results with most frequent named entities at the top.
-- Used technologies like spaCy and PySpark RDD transformations: map, flatMap, reduceByKey, sortBy.

Question 2 – Search Engine for Movie Plot Summaries
We built a two-part search engine over movie plot summaries using TF-IDF and Cosine Similarity.

Part A: TF-IDF Search:
-- Read plot summaries and metadata.
-- Removed stopwords using nltk.
-- Computed TF and IDF for terms in a search file (search_terms_oneperline.txt).
-- Mapped top movie IDs to their names using metadata.
-- Displayed top 10 documents ranked by TF-IDF.

Part B: Cosine Similarity Search:
-- Tokenized and filtered both queries and documents.
-- Computed term frequency vectors using Counter.
-- Calculated cosine similarity
-- Returned top 10 most similar movie plots to each query.
-- Used technologies like nltk for stopword filtering, PySpark for document parsing and transformation, and python standard libraries (math, functools, collections.Counter) for vector math.
