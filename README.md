# Document-based-QnA
This is a LLM-based document QnA pipeline that extracts text from a given document and provides answers to user prompts regrading the content of the document.

The pipeline was tested on a couple of documents containing information of the electoral bonds vis-a-vis the Indian General Elections, from 2019 to 2024 provided by Election Commission of India.

The "party_bonds.pdf" file contains the complete list of electoral bonds encashed by all the listed political parties between 2019 to 2024.

The "comapny_bonds.pdf" file contains the list of private/public entities that provided the bonds within the same timeline and of various denominations. Note that every bond has a unique bond number with it and hence makes tracking transactions easier in these documents.

We have performed LLM-based Named-Entity Recognition and LLM-based Query Extraction specifically to extract data from these documents and run a query-based system to tend to indiviuak user prompts based on the contents of these documents.

Provided here is a Colab notebook that can be used to access the StreamLit website where our model has been deployed. You would have to upload a couple of documents and ask questions based on the format given below.

Some sample prompts are given as follows: 

"What was the total amount received by <POLITICAL_PARTY> on 20th October 2022?"

"What was the total amount received by <POLITICAL_PARTY> by <PURCHASER_NAME> in the 
 month of July in 2021?"
