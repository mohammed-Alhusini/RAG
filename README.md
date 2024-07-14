# RAG-model-

Developing a Retrieval-Augmented Generation (RAG) on nezams (it's a legal search
engine) (https://nezams.com/). This will simplify the user journey to access legal
documents making it easier and more accurate for users to find legal information.
The chatbot will be available to all nezams users

# Design Process

• Data Preparation

• A. Raw Data Sources
o Collect raw fomr nzamez website.

• C. Chunking
o Break down the extracted information into manageable chunks that can be
processed effectively.

• D. Embedding
o Convert the chunks into numerical vectors using embedding techniques.

• Vector Database
o Store the embeddings in a vector database for efficient retrieval.
o The vector database allows for the quick search of relevant legal
information based on the query.

• Query Processing
o When a user submits a query it will convert it into an embedding.

• Retrieval of Relevant Data.
o Use the query embedding to search the vector database for relevant data.
o Retrieve the most pertinent legal information Most of the time we retrieve
the closest five from the embedded query.

• Response Generation
o Use prompt engineering to pass relevant data to LLMs for generating
coherent and accurate responses to user queries.

# Implementation

Building the chatbot involved using various frameworks and tools each chosen for
its specific strengths:

• Web Scraping: BeautifulSoup4 open-source library and it was perfect for
extracting data from legal websites.

• Embedding Models: I used the closed-source text-embedding-3-small-model from
ChatGPT to convert text into vector representations.

• Vector Databases: ChromaDB open-source vector database and it is ideal for
storing and retrieving embeddings efficiently.

• Chatbot: ChatGPT 4o its super powerful.

• UI: Gradio open source tool helped me create an interactive
and user-friendly front-end.
