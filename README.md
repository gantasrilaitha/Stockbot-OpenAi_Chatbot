# 🤖 Stockbot-OpenAi_Chatbot
A prototype of a chatbot built using OpenAi Threads &amp; Function calling mechanism for financial service providers.

## Overview
A conversational-ai bot designed to handle and understand users' queries related to services provided by the financial institutions. Appropriate runner is invoked that takes necessary parameters from user's query which then runs and returns appropriate results in response to their query. <br>
***Ex:*** if a query related to stock availability is asked, then ```stock_available function()``` is called.

## Working Process 
1. **Initialize the OpenAI Client:** Initialise the openai client using ```OpenAi API Key``` and create the Beta assisstant.
2. **Context Setting:** Set the context for the assisstant and declaring all the necessary functions appropriately.
3. **Create a Communication Thread:** Create a thread that acts as a bridge between user and assisstant, facilitating exchange of messages between them.
4. **Define Functions:** Implement the functions that were previously declared in the assisstant's context.
5. **Non-Streaming Threads:** Threads run without streaming.
6. **Function Invocation:** Appropriate function is invoked based on user's query and the response returned by the runner/function is returned to user over the same thread.

## Tech-Stack
Python, OpenAi Services


## References
  - https://platform.openai.com/docs/api-reference/introduction?lang=python <br>
  - https://platform.openai.com/docs/assistants/deep-dive/creating-assistants <br>
  - https://platform.openai.com/docs/guides/function-calling
