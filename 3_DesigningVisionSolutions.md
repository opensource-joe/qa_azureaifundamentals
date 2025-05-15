# Designing Azure AI Vision Solutions

## Azure AI Vision
- Provides computer vision.
- Does not require knowledge of ML.
- Collection of services including Image Analysis, Optical Character Recognition, Face, and Spatial Analysis.
- To use AI Vision service, create an AI Vision resource or AI services resource. AI services resources can also be used for other AI services such as language.

- Creating a custom model:
    - Choose type of model.
        - Object detection returns a list of objects.
        - Image classification returns a single category.
    - Find examples of images for training.
    - Label images.
        - Create labeling project in Azure ML.
    - Train custom model.
    - Evaluate model using unlabeled images.

- Calling the AI Vision API (this will require code)
    - Different versions have different features.
        - Version 3.2 has features that will detect landmarks, celebrities, or brand images. These features not available in 4.0.

- Spatial analysis works with videos.
    - Azure AI Video Indexer performs some of the same functions. Two services may eventually be merged.
    
## Face
- Detects faces in an image.
- Identifies the specific people in an image if the model was trained on images containing their faces.
- This is a sensitive services due to privacy concerns, so most of its features are only available to Microsoft-managed customers and partners.
- Even if part of a Microsoft-managed organization, you need to fill out a form to gain access to these features.
- Note: MS does not give police departments in the US access to facial recognition services.
- If don't have access to sensitive features then can only perform face detection.

- Face Recognition (if access to sensitive services):
    - Face identification - person's picture is compared to pictures of many people.
        - One-to-many matching where a face is matched to many people (could be used to grant access to people entering a secure building, a list of all authorized people is used for verification).
    - Face verification - person's picture is compared to a specific person's picture in a database. 
        - One-to-one matching and used by applications to grant access to one particular person (banking app that needs to verify that the person trying to access the bank account is the owner).