# Designing Azure AI Language Solutions

## Extracting Information
- AI models can extract the key points being made in a document and understand the "mood" of the text.
- They can be used for tasks such as analyzing customer reviews of your products or providing chatbots for technical support.
- Azure AI Language service is part of the Azure AI services suite.
- To use it, you need an AI services resource or an AI Language resource.

- Language.Azure.com - will need code w/ API but can try out features through browser.

- Extracting Key Phrases
    - In most cases, you wouldn't extract the key phrases from only one document.
    - You would extract them from a large number of documents and use those key phrases to gain a more general understanding across documents.
    - Examples: most common tourist attractions visited by people staying at a hotel, most common phrases across all documents to understand most important topics in them.

- In Language Studio - to find PII, use the Extract PII feature instead of Extract Named Entities feature.

- Opinion mining for sentiment analysis.

- Categories and sub-categories:
    - Helpful when you need to search for a particular type of entity.
    - Finding tourist attractions could be easier with named identities than with key phrases because you could limit the search to location entities.
    - It would be even more helpful if there were a subcategory for tourist attractions.
    - To do that, train a custom named entity recognition model (although it would require a lot of work).

## Classifying Text
- Classifying text with sentiment and language.
- Opinion mining feature provides analysis of positive and negative sentiment.

## Translating Text
- Azure AI Translator in the Azure Language Studio.
- Use the Document Translation in Azure Language Studio.

## Understanding Conversational Language
- Ways to build a Chatbot. All three options can integrate with Azure AI Bot Service.
    - Prebuilt Question Answering
        - Easiest to use.
        - Feed it a document and it will do the rest.
        - Doesn't allow you to customize the responses.
    - Custom Question Answering
        - Extracts question-and-answer pairs from your documents and lets you refine them.
        - More flexible.
    - Conversational Language Understanding (CLU)
        - Can handle more complex conversations.
        - Formerly known as LUIS.
        
- CLU model needs utterance, entity, intent, and none intent.
- Building a CLU - define schema (intents and entities), train model, deploy model, and test model. (Use the Language Studio)
- Ways to add an entity - list, learned, prebuilt, regex.

- Training and testing a model.
    - Feed model with training data, the model looks for patterns in data to help make predictions.
    - After model has gone through data run, it can only be properly evaluated by feeding it data it didn't see during the training run (now use test data) and then check the accuracy of model predictions.

- Splitting data. Split data into two groups to train a model. About 80% in training data and 20% of original data in test data set.

- To finalize Chatbot for physical functionality, it would need to be deployed with device drivers for lights and fans and it would need an interface preferably with speech recognition system.