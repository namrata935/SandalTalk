# SandalTalk
Submission for IIITB Hackathon

Overview
This project processes audio files by transcribing them into kannada text and the transcriptions and the corresponding english translations are input in a csv file called "cleaned_transcriptions_dataset.csv" . The user is prompted to upload an audio file and to select a language of the audio(english/kannada). Our model then uses semantic search to find the answer in the dataset and returns the refined answer (using T5 AI model). 

Dataset
The dataset is stored in the data folder in this repository at "cleaned_transcriptions_dataset.csv".
It contains transcription data and their corresponding translations for matching with the user-provided audio files.

Setup Instructions
Requirements
Google Colab is recommended for running the code

Python Packages:
speech_recognition
transformers
pandas
fuzzywuzzy
langdetect
google.colab
torch
ffmpeg
ipywidgets
deep_translator
pydub

Running the Project
- Open the Notebook named "sandal_mainpgm.ipynb" which you can find in the repository. this is the main file. 

- Or open this repository in Google Colab by clicking this link: https://colab.research.google.com/drive/1vHInu8bcbVavBoCqC4RKEF6YoiN3xtNO?usp=sharing

- run the code block under the label "installation of libraries" and then run the main code under the label "main code".

Upload Audio Files:

You'll be prompted to upload an audio file (Kannada or English).
Audio files will be processed for searching for the dataset. the path to dataset (locally uploaded in github) will be in the main code.
path to dataset is already in the code. so directly run it. 

Transcription and Matching:

The script will transcribe your uploaded audio into text using Google’s Speech-to-Text API.
The transcription will be matched with the dataset included in this repository for further refinement and analysis.

Refined Output:

Both Kannada and English transcriptions will be refined using a T5 model.
The refined answers will be displayed as output when the code is run. 

Note:
If your audio is in another format, it will automatically be converted using FFmpeg.

Please view the screenshots uploaded in the repository (includes examples of working of the model with kannada audio upload and english audio upload)
