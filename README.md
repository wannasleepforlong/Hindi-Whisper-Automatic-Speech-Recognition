# Hindi-Whisper-Automatic-Speech-Recognition
Transcription of Hindi audio using Whisper OpenAI 
Overview
This repository contains the implementation of the Hindi Whisper Automatic Speech Recognition (ASR) model using OpenAI's Whisper. It includes the transcription of audio files and evaluation of performance using Word Error Rate (WER). The dataset used is the Kathbath dataset.

Project Description
The project involves:

Transcription: Using the Whisper ASR model to transcribe Hindi audio files.
Evaluation: Calculating the Word Error Rate (WER) to assess the accuracy of the transcriptions.
Analysis: Analyzing errors such as substitutions, deletions, and insertions in the transcriptions.
Installation
To run this project, you need to have Python installed. You can install the required dependencies using the following commands:

bash
Copy code
pip install -U openai-whisper
pip install asr-evaluation
pip install jiwer
Usage
Download and Prepare Data: The dataset is automatically downloaded and extracted in the script.

Transcription: The ASR model transcribes audio files from the Kathbath dataset.

Evaluation: The script calculates the WER and analyzes substitutions, deletions, and insertions.

Example
To run the transcription and evaluation, execute the provided Jupyter Notebook or Python script. The results will be saved in a CSV file, and error statistics will be printed to the console.

python
Copy code
import whisper
import pandas as pd
from jiwer import wer, process_words

# Load the model
model = whisper.load_model("large")

# Transcribe audio files
# ... (code to transcribe audio files)

# Calculate WER
# ... (code to calculate WER and analyze errors)
Results
The analysis provides insights into the performance of the ASR model. The number of substitutions, deletions, and insertions are computed, and the total number of words is reported.

plaintext
Copy code
Substitutions: <number>
Deletions: <number>
Insertions: <number>
Total number of words: <number>
Note: High numbers of substitutions might indicate challenges specific to the Hindi language, including variations in spelling and pronunciation.
