# Data files for COMM3130 Group Project

This is our data folder! This folder contains all of the data that we collected and sought to analyze for our project. 

## Subfolders 

There are 5 subfolders which demonstrate our multi-step data collection process:

* **Audio_Original:** We began by converting YouTube videos of each selected interview and podcast into MP3 files for audio processing.

* **Audio:** Using Audacity, we split the full MP3 files into parts because the OpenAI Whisper Model through API has a limit of 25Mb.

* **Raw_Transcripts:** To identify and separate speakers within the audio, we employed the Picovoice model and API, which assigns speaker IDs to different segments of speech.

* **Transcriptions:** The speech from each segment was transcribed using the OpenAI Whisper model, which provides high-accuracy transcriptions for natural speech.

* **Final_Transcriptions:** To ensure the accuracy of speaker identification, we manually reviewed the original videos to label each speaker as either the candidate (Trump or Harris) or the host.

## Data
We collected data for each category: The categories are labeled within the subfolders as Trump_Podcasts, Trump_Interviews, Harris_Podcasts, and Harris_Interviews. The data is listed in the following format: Candidate_Source (i.e. Trump_Adin_Ross). If the original file was larger than 25Mb and has to be split, the number of the part is listed (i.e. Harris_All_The_Smoke_Part_2)


We collected data for each category, which is stored in clearly labeled subfolders:

* Trump_Podcasts
* Trump_Interviews
* Harris_Podcasts
* Harris_Interviews
  
Each data file is named using the following format: Candidate_Source

For example:

* Trump_Adin_Ross for a Trump podcast interview with Adin Ross.

If the original file exceeded 25 MB and required splitting, the part number is appended to the filename. For instance:

* Harris_All_The_Smoke_Part_2 indicates the second part of a split file.

This naming convention ensures consistency and makes it easy to locate and identify files based on the candidate, source, and file structure.