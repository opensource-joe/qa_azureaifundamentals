# Understanding the Azure OpenAI Service

## An Introduction to Generative AI
- OpenAI has created groundbreaking technologies like ChatGPT and DALL-E.
- technologies are built with AI models that can take natural language input from a user and return a machine-created response human-like response.
- Azure OpenAI Service is a partnership between MS and OpenAI that allows users to build enterprise-grade solutions with OpenAI models.
- Allows users to summarize text, get code suggestions, generate images for a website, and more.
- OpenAI models have several capabilities:
    - Generate natural language to summarize text, suggest alternate sentences, etc.
    - Generate code by translating from one language to another, identify bugs, etc.
    - Generate images for publication from text descriptions.

- What is Generative AI?
    - Generative AI models (e.g., GPT), are at the heart of OpenAI.
    - Understand and create natural language.
    - OpenAI's generative AI takes a prompt, returns a natural language, visual, or code response.
    - GPT models try to infer the context of the user's question based on the prompt.

- Natural Language tasks:
    - Summarizing text.
    - Classifying text.
    - Generating names and phrases.
    - Translating languages.
    - Answering questions.
    - Suggesting context.

- Responses generated are best guesses from a machine. They can be incredibly accurate but it's important to review the output of GenAI models for accuracy.

- GenAI models can create and edit images.
    - The model that works with images is called DALL-E.
    - Creates realistic and artistic images.
    - Change the layout or style of an image.
    - Can create variations on a provided image.

- Where do OpenAI Models fit in broader AI landscape?
    - AI imitates behavior by relying on machines to learn and execute tasks.
    - ML is a subset of AI where algorithms take in data and fit models to the data to make predictions.
    - Deep Learning models are a subset of ML where artificial neural networks are used to return results for more complex use cases.
    - Many Azure AI services are built on deep learning models.

## Azure OpenAI Service
- Partnership with OpenAI that leverages Azure's infrastructure to assist users in developing. Uses Azure's security, compliance, and regional availability for developing production applications. 
- Deploys OpenAI model capabilities across a range of MS products. 
- Azure powers all of OpenAI's workloads.

- Combines Azure's capabilities with OpenAI's generative AI model capabilities.
    - Pre-trained generative AI models.
    - Customization capabilities.
    - Built-in tools to detect and mitigate harmful use cases.
    - Enterprise-grade security w/ role-based access control and private networks.

- OpenAI provides its AI models to developers for building a variety of software applications.

- Support AI workloads:
    - ML
    - Computer Vision
    - NLP
    - Conversational AI
    - Anomaly Detection
    - Knowledge Mining

- Azure AI categories:
    - Azure ML Platform
    - Cognitive Services
    - Applied AI Services

- Azure Cognitive Services
    - Vision
    - Speech
    - Language
    - Decision
    - Azure OpenAI Service

- Azure's existing Language Service can be used widely known use-cases that require minimal tuning.
- Azure OpenAI's service may be more beneficial for use-cases that require highly customized generative models, or for exploratory research.

- Which model to use?
    - Time and compute needs play a role in ML training.
    - Model needs to be trained with a substantial amount of cleaned data.
    - The "learning" portion of training requires a computer to identify an algorithm that best fits the data.
    - The complexity of the task and desired level of model performance factor into the time required to run through possible solutions for a best fit algorithm.

- Azure OpenAI Studio is a platform that you can use to build AI models and deploy them for public consumptions in software applications. Different models are optimized for different tasks.

- Azure OpenAI Models
    - GPT-4 models represent the latest generative modes for natural language and code.
    - GPT-3.5 models can generate natural language and code responses based on prompts.

- Getting access to Azure OpenAI
    - Requires an application process.
    - Use the service by creating an Azure OpenAI resource.
    - Use the services through REST APIs, Python SDK, or the web-based interface in the Azure OpenAI Studio.

## The Natural Language Capabilities of OpenAI
- OpenAI's natural language models can understand and generate natural language.
- Models have been trained on a diverse range of internet text.
- Generate responses based on prompts.

Natural Lanaguage tasks:
- Summarize text
- Classify text
- Generate names or phrases
- Translate text
- Answer questions
- Suggest content

Tokens: break down input chunks of characters known as tokens.
- Tokens mapped into vectors for ML model to use for training. 
- User input is also broken down into tokens.
- Generated responses are best guesses from a machine.

When you see generative AI capaabilities in other applications, developers have taken building blocks, customized them to a use case, and built them into the back-end of new front-end user interfaces.

The model provided on the back-end is what is available as a building block with both the OpenAI API and Azure OpenAI API. You can utilize ChatGPT's capabilities on Azure OpenAI via the GPT-3.5-Turbo model.

## OpenAI Code Generation Capabilities
OpenAI's code generation AI models (GPT-4, GPT-3.5-Turbo) can understand natural laungage or code snippets and translate them into code.

Code generation capabilities - C#, Javascript, Pearl, PHP, Python.

Models can generate code based on natural language prompt. Ask it to write a Python function that adds two numbers, and the model will generate a Python function that accurately performs this task.

The generated code is a best guess from a machine.

When you see code generation capabilities in other applications, developers have taken the building blocks, customized them to a use case, and built them into the back-end of new front-end interfaces.

## OpenAI Image Generation Capabilities
OpenAI's image generation models (e.g., DALL-E) can create new images based on a prompt, a base image, or both.

Generative AI models can:
- Create a realistic and artistic image
- Change the layout or style of an image
- Create variations of a model image

Image creation in three categories:
- Image creation
- Editing an image
- Creating variations of an image

Original images can be generated by providing a text prompt of what you would like the image to be of.

The model provided on the back-end is what is available as a building block with both the OpenAI API and Azure OpenAI API.

## Azure OpenAI Access and Responsible AI Policies
Azure OpenAI provides powerful NLP models capable of completing various tasks.

Those tasked with developing and deploying AI systems should work to identify, mesuare, and mitigate harm.

Six MS AI Principles:
- Fairness - AI systems shouldn't make decisions that discriminate against or support bias of a group or individual.
- Reliability and safety - Ensure AI systems respond safely to new situations and potential manipulation.
- Privacy and security - AI systems should be secure and respect data privacy.
- Iclusiveness - Ensure that AI systems empower everyone and engage people.
- Accountability - Refers to holding people accountable for how AI systems operate.
- Transparency - Ensures that AI systems have explanations so users can understand how they're build and used.

*Transparency Notes*
Intended to help you understand how MS's AI technology works, the choices system owners can make that influence system performance and behavior, and the importance of thinking about the whole system, including the technology, the people, and the environment.

*Using AI Responsibly*
Users must submit registration to use OpenAI and change abuse monitoring settings.

### Quiz:
1. What is DALL-E? An image generation model developed by OpenAI

2. What is the relationship between AI, ML, Deep Learning, and GenAI? MS is a subset of AI, Deep Learning is a subset of ML, and GenAI is a type of Deep Learning

3. What is guaranteed to be true 100% of the time, regarding code generated by OpenAI's code generation AI models? The generated code will sometimes be syntactically or logically incorrect