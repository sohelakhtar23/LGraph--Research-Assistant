# 🧠 Research Assistant using LangGraph

This project is a **LangGraph-based multi-agent research assistant** that automates the process of researching a topic and generating a structured report. It utilizes **LangGraph**, **LangChain**, **Tavily** for web search, **Wikipedia**, and **LLMs** to simulate a team of analysts and experts working together to produce a comprehensive output.

## 📽️ Demo 
Watch the demo<br>
[![Watch the demo](https://img.youtube.com/vi/pP4EDtZEgqs/0.jpg)](https://www.youtube.com/watch?v=pP4EDtZEgqs)
---

## 📌 Key Features

- ✅ **Dynamic Analyst Creation**: Analysts are generated based on user preferences.
- 🔍 **Web & Wikipedia Search**: Uses Tavily API and Wikipedia to collect relevant information.
- 🤖 **LLM-Powered Discussion**: Analysts consult with expert LLMs to refine answers.
- 📝 **Automated Report Generation**: Generates a structured report with:
  - Introduction
  - Main Report Body
  - Conclusion

---

## 🔁 Workflow

Here is the high-level flow of the project:

![LangGraph Flow](https://github.com/sohelakhtar23/Images/blob/main/AgenticAI/LGraph%20Research%20Assistant/diag1.jpeg)

1. **Start**
2. **Create Analysts**
3. **Conduct Interview**:
   - Ask Questions
   - Search Web / Wikipedia
   - Generate Answers with LLMs
4. **Save Interviews**
5. **Write Report Sections**
6. **Finalize the Report**

---

## 📄 Sample Output

![Final Report Sample](https://github.com/sohelakhtar23/Images/blob/main/AgenticAI/LGraph%20Research%20Assistant/output1.png)

---

## 🛠️ Tech Stack

- 🧱 **LangGraph**
- 🧠 **OpenAI / LLMs**
- 🔎 **Tavily (Web Search)**
- 📚 **Wikipedia**
- 🧵 **LangChain**

---


## Setup

### Clone repo
```
git clone https://github.com/sohelakhtar23/LGraph--Research-Assistant.git
$ cd LGraph--Research-Assistant
```

### API Keys

* If you don't have an OpenAI API key, you can sign up [here](https://openai.com/index/openai-api/).
* Sign up for LangSmith [here](https://smith.langchain.com/).
* Generate a LangSmith API key.

### Set up Tavily API for web search

* Tavily Search API is a search engine optimized for LLMs and RAG, aimed at efficient, 
quick, and persistent search results. 
* You can sign up for an API key [here](https://tavily.com/). 


### Set Environment Variables

* Create a `.env` file in the root directory:
* Edit the `.env` file with the following:
```shell
LANGSMITH_API_KEY=your_langsmith_api_key
LANGSMITH_TRACING=true

OPENAI_API_KEY=your_openai_api_key

TAVILY_API_KEY=your_tavily_api_key
```

* Copy this `.env` file in the studio folder as well.

### Executing the Code

To run the LangGraph studio first goto studio folder in the terminal and then run start LangGraph studio using **langgraph dev**:
```
cd studio
langgraph dev
```

There is also a notebook **research-assistant.ipynb** file in the root directory containing all the step-by-step code with descriptions.
