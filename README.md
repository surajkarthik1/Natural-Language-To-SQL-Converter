# Natural-Language-To-SQL-Converter

Project Overview:

This repository hosts the Natural Language to SQL Converter project, designed to empower users with varying technical expertise to generate SQL queries from natural language descriptions. The project leverages state-of-the-art neural network architectures, such as T5 transformers and Large Language Models (LLMs), to translate textual input into executable SQL commands.

Background:

Many users in corporate environments lack the technical skills required to query databases directly. This project addresses this gap by allowing natural language input to be converted into SQL, making database interaction more accessible and democratizing data retrieval within organizations.

Data:

The models are trained on the WikiSQL dataset, which contains over 70,000 hand-annotated examples of questions and SQL queries covering a wide range of topics and database schemas.

Methodology:

The system implements a pipeline that includes:

* Intent Detection: Classifies the type of SQL operation (e.g., SELECT, INSERT) needed based on the user's natural language input.
* Entity Recognition: Extracts relevant database elements like table names and conditions from the natural language input.
* Token Mapping to Database Schema: Maps extracted tokens to the appropriate schema elements in the database.
* Query Generation: Constructs and outputs the SQL query based on the mapped tokens and detected intent.
  
Models Used:

* T5 Transformers: Initially used for generating SQL queries based on their ability to handle a range of NLP tasks.
* Google Gemini LLM: Implemented to enhance the accuracy and complexity of query handling. This LLM model, accessed via the Google Gemini API, demonstrated superior performance, particularly in complex query scenarios 
  involving aggregation, union, and join operations.
  
Results:
The project achieved notable success in translating natural language to SQL:

* T5 Model: Achieved an accuracy of 58.06%.
* LLM Model: Outperformed the T5 with an accuracy of 64.19%, especially effective in complex query scenarios.

Conclusion:

In conclusion, this project successfully demonstrates the significant potential of using advanced neural network architectures, specifically T5 transformers and Google's Gemini LLM, for the task of converting natural language queries into SQL statements. The application of these technologies has proven to not only enhance the accessibility of databases to non-technical users but also improve the efficiency and accuracy of query generation.

Our findings indicate that while the T5 model provides a robust foundation for understanding and generating SQL queries, the Gemini LLM excels in handling more complex queries and achieves higher accuracy. This underscores the value of incorporating cutting-edge language models to tackle sophisticated natural language processing challenges. This project not only advances the field of database querying but also sets the stage for future innovations that could revolutionize how users interact with data systems across various industries.

