# llm-rag
### 1.1 Building an RAG application 

implement a simple RAG pipeline to answer questions about the FAQ Documents from Zoomcamp courses

What we will do:
Create a Q&A system for answering questions about these documents

Index Zoomcamp FAQ documents


### 1.2 Preparing the Environment
pip install tqdm notebook==7.1.2 openai elasticsearch pandas scikit-learn 

### 1.3 Retrieval
A customed search engine was created as minsearch - https://raw.githubusercontent.com/DataTalksClub/llm-zoomcamp/main/01-intro/minsearch.py

### 1.4 Generation with OpenAI
Invoking OpenAI API
Building the prompt
Getting the answer

### 1.5 search with elasticsearch 
Run ElasticSearch with Docker
Index the documents
Replace MinSearch with ElasticSearch
--running the elasticsearch in codespace
docker run -it \
    --rm \
    --name elasticsearch \
    -p 9200:9200 \
    -p 9300:9300 \
    -e "discovery.type=single-node" \
    -e "xpack.security.enabled=false" \
    docker.elastic.co/elasticsearch/elasticsearch:8.4.3

