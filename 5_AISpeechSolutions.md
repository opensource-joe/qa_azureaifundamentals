# Designing Azure AI Speech Solutions

## Speech to Text
- Azure AI Speech
    - To use the AI Speech service, you need:
        - An AI Speech resource
        - An AI services resource
- To add AI Speech features to your applications, you need to write code that calls the service's API. 
- Try out speech features on the web at [speech.microsoft.com](https://speech.microsoft.com/portal).
- Examples
    - Videos that need captions either recorded or live (harder to do).
        - Offline captioning - captions start immediately (no lag like w/ live), captions are nicely formatted, and there can be a phrase list which are a list of words that you expect to be in your content.
    - Call center for transcript - uses batch transcription component, uses speaker separation. Speaker separation in the API is called diarization, for recognizing specific speakers use Speaker Recognition but it requires you to train a model using audio samples from the people you want to identify. Also uses batch transcription, speaker separation, conversation PII, sentiment analysis, and call summarization.

## Text to Speech
- Chatbot - need speech to text and text to speech. Azure AI Speech service provides both of these capabilities. Text to speech allows you to pick the voice.
- Can create own voice with Custom Neural Voice feature. This could be used for nefarious purposes to imitate someone else. 
    - MS strictly controls the use. 
    - Only available to MS-managed customers who register to use the service and only for specific use cases.
    - Many companies use custom voices so their applications don't sound like other company applications. They want their company to be represented by a unique voice that reflects their branding.

## Speech Translation
- Convert speech in one language to speech in another language.

### Quiz
1. If you wanted to use the Azure AI Speech service to add subtitles to an existing video, and you needed it to accurately spell the names of your company's products, which two features would you need to use? (Choose two answers.)
- Phrase list
- Offline captioning

2. Which feature is part of the Batch Transcription API in the Azure AI Speech service?
- Speaker separation (diarization)

3. Which feature of the Azure AI Speech service is only available to Microsoft-managed customers who register to use it?
- Custom Neural Voice