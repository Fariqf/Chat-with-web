# Chat-with-web
This Streamlit application allows you to interactively chat with a website. You can input a website URL and ask questions, and the system will retrieve relevant information from the website to answer your queries.

## Getting Started
### Prerequisites
1. Python 3.7 or later
2. Streamlit
3. langchain
4. dotenv

### Installation
1. Clone this repository:
   git clone https://github.com/Fariqf/Chat-with-web.git
   cd Chat-with-web
   
2. Install the required packages:
  pip install -r requirements.txt

3. Create a .env file in the root directory with the following content:
   OPENAI_API_KEY=your_openai_api_key

4. Run the Streamlit app:
   streamlit run app.py

## Components
### Website Data Retrieval
The application retrieves data from the specified website using a WebBaseLoader. It then splits the loaded data into chunks for processing.

### OpenAI Embeddings and Chroma Vector Database
The loaded data is processed with OpenAI embeddings, and a Chroma vector database is created. This database facilitates efficient document retrieval based on the provided query.

### Chat With Website
The system uses the ChatOpenAI model (gpt-3.5-turbo) to interactively answer questions based on the information retrieved from the website.
