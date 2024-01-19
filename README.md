# General Description
This repository contains a corpus in the format of CSV, a most-played list of Coldplay on Spotify in CSV, and a Jupyter Notebook file regarding the data scraping, cleaning, and tagging processes, aiming to display the process of creating a corpus. Due to copyright issues, the lyrics file has not been uploaded.

# Purpose of the corpus
This corpus is designed to explore the language style and emotional characteristics of the lyrics of Coldplay's top 20 most-played songs on Spotify until December 18, 2023, from the perspective of part-of-speech and lemmas.

# Criteria for Text Selection:
- **About the text**: 
The texts are Coldplay's top 20 most-played songs on Spotify until December 18, 2023.
- **Why Spotify and Kworb**: 
Kworb is a data-centric website providing up-to-date charts and analytics on music trends across major streaming platforms like Spotify, Apple Music, and YouTube. The top 20 songs on Spotify were chosen because Spotify is one of the world's largest music streaming service providers, with a broad user base. 
- **Where and how to get the Text**: 
The texts were copied from the official website of Coldplay.

# Scraping (Collecting) Process
- **Scraping the most-played list from Kworb**: Pandas, BeautifulSoup, Requests in Python were used to send requests to Kworb for ranked, structured data with song names, total streaming counting, and daily streaming counting of Coldplay's songs on Spotify until December 18, 2023. The structured data is saved in CSV format. 

# Cleaning Process
- Lowercasing
- Removing punctuation
- Tokenization

# Tagging Process:
- Utilizing the POS function in Spacy to get the POS of tokens.
- Utilizing the lemma function in Spacy to get the lemmas of tokens.

# Format of Corpus 
CSV

# Varibles of Corpus
| Variables       | Description            | Data Type    |
|-----------------|------------------------|--------------|
| filename        | name of the song       | string       |
| original_text   | original text          | string       |
| tokens          | tokens of the text      | string       |
| POS             | part of speech of tokens| string       |
| lemmas          | lemmas of tokens        | string       |

# Source
https://www.coldplay.com/
https://kworb.net/spotify/artist/4gzpq5DPGxSnKTe4SA8HAU_songs.html
