## Data Analysis Notebooks

This folder should contains the Jupyter notebooks in which we perform the text analysis on the podcasts transcripts. It includes the following python notebooks:

- **00_transcription_and_diarization.ipynb**: Transcribes audio files (mp3) of interviews and podcasts using the OpenAI Whisper model, with diarization for speaker identification via the Picovoice API. The notebook handles the processing of audio files and manages file size limits for transcription.

- **01_data_processing.ipynb**: Aggregates and organizes podcast and interview transcripts into a structured list of dictionaries. Each dictionary includes metadata like title, medium, speaker-specific transcripts, and a list of tokens for further analysis.

- **02_frequency_lists.ipynb**: Analyzes the frequency of words and bigrams in Trump and Harris interviews and podcasts. The notebook covers data preparation, token frequency lists, bigram frequency lists, and comparative analyses of the two candidates’ language usage.

- **03_keyness_analysis.ipynb**: Conducts keyness analysis to compare word frequency differences between Trump and Kamala's podcasts and interviews. It includes statistical measures (e.g., Keyness, % Diff, and BIC) to identify significant disparities in language use between the two candidates across different formats.

- **04_kwic_analysis.ipynb**: Performs Key Word in Context (KWIC) analysis to explore how specific words are used in context within the Trump and Harris interviews and podcasts. The notebook provides detailed steps for generating, visualizing, and interpreting KWIC data for various linguistic analyses, including issue focus, opponent mentions, and emotional language.

- **05_dispersion_plots.ipynb**: Creates dispersion plots to visualize the frequency and distribution of topics across the interviews and podcasts. The notebook includes the creation of topic lists and overlayed plots to observe where specific topics are discussed, and compares the sparsity of topics across different interviews.

- **functions.ipynb**: Contains reusable functions for tasks like KWIC generation, sentiment analysis, and other analysis steps. This notebook centralizes key functions used across other analysis notebooks for modularity and code efficiency. 




