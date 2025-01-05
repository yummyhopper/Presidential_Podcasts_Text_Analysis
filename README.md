# Text Analysis of Presidential Podcasts 

*By Max Orenstein & Julia Keswin*

<img src="cover_image.avif" alt="Cover Image" width="1200"/>

Traditional media (e.g. debates, press coverage, and formal interviews) has long been a cornerstone of presidential campaigns, shaping how candidates are perceived by the public. However, in 2024 we saw a shift towards new media for where people got their election news. Some even went as far as to deem 2024 the "Podcast Election" due to both candidates appearing on several popular political and entertainment podcasts. 

These podcasts allowed both Kamala Harris and Donald Trump to reach broader audiences who may have been less engaged with mainstream news. In this analysis, we will explore how each candidate communicates through podcasts compared to traditional outlets, examining their tone, messaging strategies, and audience engagement to uncover the evolving dynamics of political communication. Our dataset comprises transcriptions from four distinct categories: Trump podcasts, Trump interviews, Harris podcasts, and Harris interviews. 

## Key Research Questions

* Opponent Mentions: How often does Trump mention Harris in news interviews versus podcasts and vice versa?
* Emotional Language: How does the frequency of emotional language used by Kamala Harris and Donald Trump differ between podcasts and formal news outlets?
* Structural Analysis: How many turns/how are topics covered in news interviews versus podcasts?
* Audience Engagement: How do Trump and Harris modify their language to engage with different audience demographics across podcasts versus news interviews?

## Analysis Methods + Tools

This project was done 100% in Python and includes the following analysis methods:

* Audio Transcription and Diarization: Using Picovoice Falcon on top of OpenAI's Whisper model we transcribed interview and podcast mp3 audio files into .txt files diarized for speaker. 
* Data Structuring: We aggregated the transcriptions into a list of dictionaries with keys for transcription title, medium, transcription (stored in tuples), and tokens.
* Frequency Analysis: Using counter objects we looked at token and bigram frequencies for key terms.
* Keyness Analysis: We statistically analyzed which words were being used more in interviews vs podcasts for each candidate relative to corpus size.
* Key Words In Context (KWIC) Analysis: Choosing key words to analyze, we looked at the context those words were being used in for each candidate. 
* Dispersion Plots: Charting where each candidate says certain types of words in each of their interviews and podcasts. 
* Sentiment Analysis:

## Contents

This repository includes the following folders: 

* The "data" folder contains our original audio, audio (split into parts for processing), raw transcripts, and our final transcriptions.
* The "data_analysis" folder contains all of the different methods we used to analyze the the data.
* The "data_story_output" folder contains a simplified final data story.
* The "presentation" folder contains a brief PowerPoint presentation of our project and some initial findings we had at the time of creating the slides. 

## Data Sources

The data we used for this project were mp3 files we converted from YouTube videos using tools like https://ezmp3.cc/. The podcasts and interviews we used were: 

- **Trump Podcasts:**
  - Nelk Boys
  - Theo Von
  - Bussin with The Boys
  - PBD
  - Flagrant
  - Lex Friedman
  - Adin Ross
  - Elon Musk
  - Logan Paul
  - Ben Shapiro
  - Joe Rogan

- **Harris Podcasts:**
  - Howard Stern
  - Breakfast Club
  - Club Shay Shay
  - Call Her Daddy
  - All the Smoke

- **Trump Interviews:**
  - Bloomberg
  - Fox News Harris Faulkner
  - Fox News Laura Ingram
  - NABJ Conference

- **Harris Interviews:**
  - Fox News
  - 60 Minutes
  - CNN
  - NBC
