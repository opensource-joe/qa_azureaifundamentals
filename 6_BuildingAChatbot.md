# Building a Chatbot on Azure

TODO: Follow videos and create a Chat Bot

[GitHub repository for ChatBot](https://github.com/cloudacademy/azure-chatbot)

## AI Services in Azure
- Azure Bot Service
- Azure AI Services - Vision, Speech, Language, and Knowledge
    - These services let you add AI capabilities even if you don't know anything about ML.
    - CLU - Conversational Language Understanding - can be used to help bot to better understand messages received from users.
    - Question Answering - let's you create a knowledge base from questions and answers.
    - Speech Service - used to add chat capabilities to a bot.

## Question Answering
- Steps to create a bot
    1. Build a knowledge base (using question answering service).
    2. Create a bot that uses the knowledge base.

- Alternate Questions
    - Different ways of asking the same questions.
    - The services is pretty good at figuring out alternatives.
        - If the bot doesn't give you the expected answer, then you could add that phrasing as an alternate question.

- Follow-Up Prompts
    - Allow you to create multi-turn conversations.

- Metadata
    - Allows client applications to filter answers based on certain criteria.
    - You can separate project for each value of the attribute with two distinct knowledge bases - might be easier to add metadata tags.

- Can look at confidence score to see how close the answer is to the question. Can add alternate question to knowledge base.

- Don't have to add Alternate Questions, the application will watch the interaction between the user and the bot and continually update the knowledge base. The application will make suggestions and you can decide to add or not.

## Creating a Bot
- Follow the video.

## Creating a Web Chat App
- Develop using Visual Studio then embed Chat Bot code w/ secret key for chat bot authentication.
- Can use App Service and other known common apps (e.g., LinkedIn, Facebook).

## Enabling Speech
- To make production ready by working in all browsers:
    - Create an instance of the Speech Service
    - Create a Direct Line Speech channel in the Bot
    - Connect it to the Speech Service created
    - Make sure app has Web Sockets enabled so the Bot can communicate with the Direct Line Speech channel
    - Select Enable Streaming Endpoint in the Bot's configuration
    - Add code to Bot that uses Speech SDK with speech recognition and speech synthesis
    - Code will have to authenticate with Speech Service first
    - Retrieve token from Speech Service (to avoid exposing Secret Key)
    - The token would expire after 10mins so a hacker can't access Speech Service after that
    - Learn more online ;-)

### Quiz
1. To add support for spoken input and output to your Azure AI Bot Service, which of the following are required?

- Select "Enable Streaming Endpoint" in your bot's configuration
- Create a Direct Line Speech channel in your bot
- Create an instance of the Speech service

2. Which feature of the Azure question answering service allows client applications to filter answers based on certain criteria?

- Metadata

3. Which feature of the Azure question answering service allows you to create multi-turn conversations?

- Follow-up prompts