This readme file was generated on [2025-11-04] by [Maria Lodhi]

GENERAL INFORMATION

Title of Dataset: Word Frequency Spotify Dataset

Author/Principal Investigator Information
Name: Maria Lodhi
ORCID:0009-0008-2584-8629
Institution: Queen Mary University of London
Address: Mile End Road, Bethnal Green, E14NS
Email:bb25077@qmul.ac.uk


Date of data collection: (2025-11-03)
Geographic location of data collection: Data was taken from Kaggle.com, which is an online source.
Information about funding sources that supported the collection of the data:This dataset was created as part of academic coursework for LIN7078 Data Report 1. No external funding was received.


SHARING/ACCESS INFORMATION

Licenses/restrictions placed on the data: NO
Links to publications that cite or use the data: No publications currently cite this derived dataset as it was newly created for academic coursework.
Links to other publicly accessible locations of the data: https://github.com/marialodhi1054/Word-Frequency-Spotify-Dataset
Links/relationships to ancillary data sets:This dataset is derived from two Kaggle datasets focused on Spotify track information.
Was data derived from another source?
If yes, list source(s): Yes
1. Muhammad, I. (2023). "Audio Features and Lyrics of Spotify Songs." Kaggle.
Link: https://www.kaggle.com/datasets/imuhammad/audio-features-and-lyrics-of-spotify-songs
2. Pandya, M. (2023). "Spotify Tracks Dataset." Kaggle.
Link: https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset?select=dataset.csv
Recommended citation for this dataset:
Lodhi, Maria. (2025). "Word Frequency Spotify Dataset". https://github.com/marialodhi1054/Word-Frequency-Spotify-Dataset

DATA & FILE OVERVIEW

File List: 
	1.final_spotify_dataset.tsv

	2.readme_file.txt 

METHODOLOGICAL INFORMATION

Description of methods used for collection/generation of data:This is a derived dataset created by merging and processing two existing Kaggle datasets. The original data was collected by the Kaggle dataset authors.

Methods for processing the data:

1. Downloaded two source datasets from Kaggle

2. Loaded datasets into R using data.table package

3. Identified common key (track_id) for merging

4. Performed inner join to combine datasets

5. Removed duplicate entries

6. Selected relevant columns for linguistic analysis

7. Calculated word frequency metrics from lyrics

8. Renamed variables for clarity

9. Filtered to approximately 700 observations

10. Saved final dataset in tidy TSV format

Instrument- or software-specific information needed to interpret the data:

1. R version 4.3.0 or higher

2. Required R packages: data.table, dplyr, readr, stringr

3. Text editor or spreadsheet software for viewing TSV files

Describe any quality-assurance procedures performed on the data:

1. Verified merge integrity by checking track_id consistency

2. Removed duplicate songs based on track_id

3. Ensured word frequency calculations were accurate

4. Validated numeric ranges for audio features

5. Confirmed dataset follows tidy data principles

6. Checked for and handled missing values appropriately

People involved with sample collection, processing, analysis and/or submission: Maria Lodhi- Data processing, analysis, documentation, and dataset creation.

DATA-SPECIFIC INFORMATION FOR: final_spotify_dataset.tsv

Number of variables:17
Number of cases/rows:700
Variable List:
track_id : Unique identifier for the song track
song_name: Name of the song
song_lyrics: Full lyrics of the song
popularity: Popularity score of the song (likely from Spotify)
album_name: Name of the album the song belongs to
release_date: Release date of the song
genre: Genre of the song
artist: Name of the artist or band
total_words: Total number of words in the lyrics
unique_words: Number of unique words in the lyrics
lexical_diversity: Ratio of unique words to total words
love_freq: Frequency of the word "love" per 100 words
heart_freq : Frequency of the word "heart" per 100 words
you_freq: Frequency of the word "you" per 100 words
i_freq: Frequency of the word "i" per 100 words
baby_freq: Frequency of the word "baby" per 100 words
night_freq: Frequency of the word "night" per 100 words

Missing data codes: "NA" is used to indicate missing or unavailable data