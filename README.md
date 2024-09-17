<div align="center">

# PDF Analyzer usign pathway and RAG
</div>

Pathway's **LLM (Large Language Model) Apps** allow you to quickly put in production AI applications which offer **high-accuracy RAG at scale** using the most **up-to-date knowledge** available in your data sources.

This LLM App is connected to GDrive and watch for any changes (upload/delete of PDF's) happening in the folder and accordingly trains the LLM giving the most up-to-date answer based on provided data.


## How to run the project
First, clone the repo and **cd to /examples/piplines/gpt_4o_multimodal_rag** and run **docker built -t rag .** then run **docker run -p 8000:8000 rag**. Wait for processes to finish and Make a post request to http://localhost:8000/v1/pw_ai_answer with:

Headers:
Accept - */*
Content-type - application/json

body:
{
  "prompt":"type your question here"
}

