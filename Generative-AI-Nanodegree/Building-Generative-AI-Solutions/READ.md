# This is the repository for the project code of the exercise of module 5 - Building Genrative AI Solutions

**The functionalyties of this application are:**

**Generating Real Estate Listings with an LLM**

This project starts by prompting chatgpt 3-5 - Turbo to do Synthetic Data Generation, creating realistic real estate listings containing facts about the real estate. In a real life situation this would be the listing that the real estate agency has to sell.
Creating a Vector Database and Storing Listings
Then it uses lancedb, a vector database, and the class “Lance Model” to create a representation of a listing and store the information about the listings in the database.

**Semantic Search of Listings Based on Buyer Preferences**

After the application presents a user interface, built with “ipywidgets”, to get the input from the user. Here the user can specify some structured data (like for example the maximum price he wants to pay) but also unstructured data, inputting information about what he wants in natural language.
Then with this information the application performs a semantic search based on given buyer preferences. The search returns the top 5 listings that closely match the input preferences.

**Logic for Searching and Augmenting Listing Descriptions**

Now with the user input and the context from the top 5 listing previously mentioned, the application makes another call to the LLM model and uses LLM augmentation to personalize the recommended listing without changing factual information.

**Use of LLM for Generating Personalized Descriptions**

The call to model also generates a personalised description for the real estate listing that was selected  based on buyer preferences
