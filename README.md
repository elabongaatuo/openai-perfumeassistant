# Perfume Recommendations Using OpenAI API
## Imagine having a virtual perfume assistant, instead of sniffing a lot of concoctions. Well, I played around with OpenAI API and used perfume data that I had scraped for my simple recommender system,which you can find [here](https://nukato-front.onrender.com). It may not be perfume shazam, but it's a great place to start!

# Introduction
An AI perfume recommendation assistant. Allow me use an analogy, you have a shop, well stocked, you have a shop assistant. You should be able to sell right? Right. Well customer service is crucial too. In this project, the stock is the perfume data, the shop assistant is the OpenAI model and the customer service are the instructions we give the model.

# Technologies Used
1. Python 3.11.1 -  a popular programming language
2. Jupyter Notebook -  a server-client application that allows editing and running notebook documents via a web browser
3. OpenAI API - an api  that allows for any task that involves understanding or generating natural language or code using the same technology chatgpt3 is based on
4. PineCone - a fully managed vector database that makes it easy to add vector search to production applications.

# Project Flow
1. Load dataset
2. Perform tokenization -(split paragraphs/sentences into smaller units that can be assigned meaning)
3. Choose preferred model according to need and get embeddings
4. Save embeddings to vector database that allows for indexing and eliminates need for constant generation
5. Create context for AI
6. Define function that instructs how the model should respond to queries



# Installation and Usage
### The following are terminal instructions:
``` # clone repo ```<br>
``` git clone https://github.com/elabongaatuo/openai-perfumeassistant.git ```<br>
``` # change into directory ```<br>
``` cd openai-perfumeassistant ```<br>
``` # install the necessary packages ```<br>
``` pip install -r requirements.txt ```<br>

### Accessing the necessary APIs :
To access the OpenAI API, you need to create an account [here](https://rb.gy/ifuche) <br>

To access the PineCone Index API, you need to create your account [here](https://rb.gy/jshent)


# Known Issues / Disclaimer
You may obtain the API Keys from OpenAI but however may not get a response and get a **_"you exceed your current quota"_** error.<br>
To solve this, you may need to [add a payment method](https://platform.openai.com/account/billing/payment-methods).<br>
After adding a payment method, go ahead and create a new API Key. <br>
You should as well be wary of the number of tokens your dataset has as each token is charged based on the model used.<br> 
<br>
You may as well encounter an error: **_"The server had an error while processing your request. Sorry about that!"_** . Not to worry, that isn't your fault, there could be many requests from other users at the time. Here are some of the suggested solutions from the [community](https://rb.gy/ozxzvh)<br>

At the time of publishing, all keys used in the notebook have been revoked.<br>


# Resources & References
1. This amazing walkthrough/demo [medium article](https://rb.gy/4oqx4k).
2. OpenAI [types of models](https://platform.openai.com/docs/models/overview)
3. A little perfume theory - [Nukato](https://nukato-front.onrender.com)
4. OpenAI [Embeddings Tutorial](https://platform.openai.com/docs/tutorials/web-qa-embeddings)

#  Future Improvements
More information such as user feedback on perfume sillage and preference accompanied by<br>
descriptive reviews may help in better recommendations.

# Files
1. perfume-recommenderv2.ipynb - details how to go about the project
2. marashi-babbage.parquet -  contains perfume data in parquet form. (flat column data storage)
3. marashi-mapping.json -  json file that will allow for reverse mapping by index


# Author
Elabonga Atuo <br>
Contact me via [email](elabongaatuo@gmail.com)



