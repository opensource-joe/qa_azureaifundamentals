# Designing Responsible Generative AI

## MS's Six Principles of Responsible AI
- Fairness - AI systems shouldn't make decisions that discriminate against or support bias of a group or individual. (Loan application)
- Reliability and safety - Ensure AI systems respond safely to new situations and potential manipulation. (Autonomous vehicles, robots, medical diagnostics)
- Privacy and security - AI systems should be secure and respect data privacy. (people's information, obtaining permission for data capture)
- Iclusiveness - Ensure that AI systems empower everyone and engage people. (all types of people, gender, visually impaired, train model on diverse data)
- Accountability - Refers to holding people accountable for how AI systems operate. (taking responsibility, framework of guiding principles, AI not doing anything illegal)
- Transparency - Ensures that AI systems have explanations so users can understand how they're build and used. (being open how a model works, explanations for making decisions)

## Four Stages
GenerativeAI can be dangerous, especially when it gives inaccurate information.

Even when it gives accurate information, it can be harmful if it is being used for unethical purposes.

MS recommends a four-stage process when developing a GenAI application.

1. Identify potential harms
- Realize what could be harmful - say something offensive or discriminatory, give inaccurate information, support unethical behavior.
- Prioritize the harm - rank from worst to least harmful, estimate how likely it is for each type of harm to occure, Azure OpenAI has default filters in place to prevent offensive or discriminatory responses, so they're less likely.
- Test application to see if generates any harms. Use a red team to try out the system.

2. Measure potential harms
- Testing should be automated.
- Set up a measurement system used in third stage.

3. Mitigate potential harms
- Model layer
    - Select an appropriate model, such as GPT-4.
    - You could also fine-tune the model by creating a custom version that is trained with your own data, but this an expensive and time-consuming process.
- Safety system layer
    - Configure the AI platform to be more restrictive.
    - Azure OpenAI Service has content filters that can be set to different levels.
- Metaprompt and grounding layer
    - Specify information to be added to every prompt written by a user.
    - Azure OpenAI, the metaprompt is called the system message.
    - Set parameters to limit prompt context.
    - Another option is to use grounding data. Like using product information about company cars.
    - Azure OpenAI uses Retrieval Augmented Generation (RAG) to add your data to user prompts. Azure OpenAI searches for relevant information in your data using the AI Search service, and then it adds the information if finds to the prompt.
- User experience layer
    - Place helpful hints in the user interface to help users write good prompts.
    - Let users know that the Chatbot's responses may not be accurate or helpful.
    - Can also build in a message filter to not display bad information to users.

4. Operate the solution responsibly
- Review compliance requirements.
- Create a way for users to give feedback.
- Create a way to block harmful responses when they are reported.
- Create a way to block users or applications that are abusing the system.
- Create an incident response plan.
- Create a rollback plan.
- Create a monitoring system.
- Release the application to a small subset of users before releasing it broadly.

## Azure OpenAI Demo
Create filters to allow or block specific types of content.

Use data files to populate Chatbot based on own data.

### Test
1. If you ensure that your AI application can be accessed by people with impaired vision, which principle are you following? Inclusiveness

2. What are two Azure OpenAI features you can use to automatically add information to user prompts? Use your own data, System prompt

3. Which is these is not one of the four stages in MS's recommended process for developing and implementing responsible AI when using generative models? Eliminate potential harms

### Additional Coursework
- [Understand text analytics](https://learn.microsoft.com/en-us/training/modules/analyze-text-with-text-analytics-service/2-understand-text-analytics)
- [Introduction to GenAI concepts](https://learn.microsoft.com/en-us/training/modules/fundamentals-generative-ai/)