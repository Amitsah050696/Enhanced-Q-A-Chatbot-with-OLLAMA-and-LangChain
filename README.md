**Enhanced Q&A Chatbot with OLLAMA and LangChain**
This project implements a simple yet powerful Q&A chatbot using LangChain, OLLAMA, and Streamlit. The chatbot allows users to ask questions, and it generates contextually relevant answers using a large language model (LLM). The backend LLM model is powered by OLLAMA, while LangChain is used for prompt management and response generation.

**Key Features:**
Interactive Interface: Built with Streamlit, this app provides a user-friendly web interface to interact with the chatbot.

Dynamic Prompting: Uses LangChain's ChatPromptTemplate to create dynamic conversation prompts that guide the language model’s responses.

LLM Integration: Leverages OLLAMA for generating high-quality responses to user queries.

Environment Variables: Sensitive information such as API keys is securely loaded via the dotenv library, ensuring scalability and security.

**How It Works:**
User Input: Users enter their question in the input box on the Streamlit interface.

Prompt Generation: The input is passed into a ChatPromptTemplate, which defines the system's and user's conversational roles.

Model Invocation: The question is sent to the selected model (e.g., "gemma3" or "gpt-4") via the OLLAMA model wrapper.

Response Parsing: The model's output is parsed and returned to the user.

**Libraries Used:**
LangChain: A framework for building powerful applications with large language models.

OLLAMA: A language model API used to generate responses to user queries.

Streamlit: A framework for quickly building and deploying data applications with Python.

dotenv: A module that loads environment variables from a .env file for secure key management.

**Customizations**:
Model Selection: You can select different models available from the OLLAMA API via a dropdown in the sidebar.

Temperature & Tokens (Future Implementation): You can add more customization for temperature and max tokens for response generation if needed.

**Environment Variables:**
LANGCHAIN_API_KEY: Your LangChain API key (required for tracing and access to LangChain features).

LANGCHAIN_TRACING_V2: Set to "true" for LangChain API tracing.

LANGCHAIN_PROJECT: The name of your LangChain project for tracking purposes.

*Troubleshooting:**
Make sure your .env file contains a valid LANGCHAIN_API_KEY.

If you see errors related to model selection, ensure the model name is correct and supported by the OLLAMA API.

If the app doesn't start, ensure all dependencies are installed and your Python environment is set up properly.

