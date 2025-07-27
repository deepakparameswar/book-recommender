pip install kagglehub
pip install pandas
pip install matplotlib
pip install python-dotenv
pip install seaborn
pip install langchain-community
pip install langchain-openai
pip install langchain-chroma
pip install transformers
pip install gradio
pip install notebook
pip install ipywidgets
pip install sentence-transformers

Vector search
-------------
once we have clean dataset we can create an vector from a raw text
once we capture the meaning of the text then we can compare how similar or different pieces of the rext are
then we bundle those vectors into a database allowing us to efficiently find the most similar books to query

1) word embeddings
   ---------------
    lets teke 7 words
   1) Queen
   2) Girl
   3) woman
   4) king
   5) boy
   6) man
   7) tree
    we can plot the above words in a 3 dimension space(see the image)
    And we can see from the image the woman and man together and 
    king and queen together and girl and boy together
    in 3 dimension second image we can see the similarities of each words in each dimensions and this is called as word embedding
    they represent meaning of the word by grouping words that are similar and by creating distance b/w words those are dissimilar
   
    one of the word embedding model is word2vec
    
    We can see one image that is the RoBERTa-Encoder-Model there we will attach CLC token at start and SEP token at the end to indentify the start and end of the sentence
    RoBERTa model build to find the masked(missing) word in an sentence  
    
    Check the Books-Embedding images there we can find how we can search for an book that are related to Roman Empire using the vector
    Here we are doing linear search and its not efficient because if our vector database is large there we need to compare our query with every vectors and its not efficient
    to solve this issue there are many other algorithms are available see Vector-indexing image
    
    in order to work with vector search we are going to work with framework called LangChain
    Also langchain provided multiple LLM models like openAI and all
    
    
2) 