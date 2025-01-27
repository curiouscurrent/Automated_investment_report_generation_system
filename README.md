# Automated_investment_report_generation_system

## STEPS FOLLOWED : 
1. Load and format mutual fund data into retrievable documents. (Each row is
converted to a Document object by Langchain)
2. Generate numerical vector embeddings for documents using a Hugging Face
embedding model. (default model used)
3. Load and configure Zephyr-7b-beta LLM with memory-efficient settings. (using
4-bit quantisation for using less gpu memory)
4. Define a structured prompt template for LLM input
5. Retrieve the top 5 documents most relevant to the query. (by performing semantic
similarity search between the document embeddings and query embedding to get
the relevant documents and selecting top5)
6. Combine retrieval and text generation for answers. ( use the top5 unique relevant
documents content to form a context and send it as an input to
Zephyr-7b-beta(text-generation) model to generate summary)
7. Next is querying and response generation for recommendations

## DEMO WORKING :

## TEMPLATE : 

![image](https://github.com/user-attachments/assets/9bbfee08-96c5-4a8b-b73b-e884b6755a6c)
![image](https://github.com/user-attachments/assets/0117f5dd-3bbc-438b-8810-c4cf308a49b2)

## QUERY AND ANSWER : 

![image](https://github.com/user-attachments/assets/8ecf4976-4277-436f-afc8-da01e48bbd93)
![image](https://github.com/user-attachments/assets/8d3a2074-5fab-4cd9-84f8-65c703aa24f0)
![image](https://github.com/user-attachments/assets/f88d0632-6b0a-4c42-a25b-be4e30c773e1)
![image](https://github.com/user-attachments/assets/c02b8205-dc55-428e-8da6-8ef9af2f7e12)
![image](https://github.com/user-attachments/assets/8b615258-b7e8-4002-a718-9fd60a18b65e)
![image](https://github.com/user-attachments/assets/b4d75372-5311-4962-ae49-852ded4ad6e9)







