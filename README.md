# DSCI 511: Data Acquisition and Pre-Processing

## _Term Project_: Song Data Mining

#### Our Team (Group 8):
> - Harsh Bolakani hvb36@drexel.edu
> - Greg Morgan gm655@drexel.edu
> - Trevor Pawlewicz tmp365@drexel.edu

---
We will explore the area of music and lyrical content to find trends in popular music according to genre.
We will ask if popular hit music (chart ranking and top selling songs) have trends in the following way:
- Are there common words and/or phrases?
- Are the common themes?
- What words can be used in a specific genre to write a popular song lyric?

We would like to give developers a dataset to create phrases to help write a popular song in a specific genre.

---
#### Potential Users and Applications:
> - Create inspiration for musicians.
> - Help musicians over creative road-blocks.
> - Assist content producers in creating the perfect song to fit their needs.
> - Looking at trends in genres to collect a dataset for lyrical inspiration.
>
> For an audience of…
> - Musicians
> - Writers
> - Producers

---
#### Source of Data:
Musixmatch ![Musixmatch logo](images/Monogram_Primary.png "Musixmatch")
Genius ![Genius logo](images/Genius.png "Genius")

---
#### Building the Dataset:
> 1. Register for an API key (musixmatch)
> 2. Retrieve song list and genre metadata from API (musixmatch)
> 3. Scrape Lyric Data with Beautiful Soup (genius)
> 4. Collect and Merge Data
> 5. Process Data
> 6. Remove Stop Words
> 7. Output the Dataset

---
#### Preprocessing Our Data:
> 1. Get the track genre.
> 2. Skip songs we didn't get lyrics for.
> 3. Tokenize lyrics and remove punctuation.
> 4. Remove any remaining punctuation from the count.
> 5. Diction where a Genre points to a list of word/count tuples sorted by the highest count.
> 6. Check top 5 words in each genre.
> 7. Remove Stop words.
> 8. Output dataset to JSON file.

---
#### Distribution Approach:
> JSON file hosted on GitHub, here in this repo:
> `FinalProject/data/word_count_by_genre.json`
> `FinalProject/data/word_count_by_genre_stop.json`

---
#### Discussion of Access Rights:
> - No Access rights (Output dataset as JSON file hosted in a Public GitHub Repository.)
> - Open to public consumption
> - We are not Publishing entire lyrical data.
> - Word counts vs. Copyrighted Lyrics

---
#### Issues and Limitations:
> ##### _Musixmatch_:
> - Limited to 2k API Calls daily
> - Free testing plan for evaluation only
> - Access to ONLY 30% of lyrics per song
> - Understanding which part of the song (beginning, middle, end) contains the lyrics that are needed to be best analyzed for our dataset.
>
> Genius.com was web scrapped to get full lyrical content of songs as a solution to only having access to the __musixmatch__ free 30% of lyrics per song.
> - Web scrapping decreased our dataset collecting performance.


---

![Drexel logo](images/Drexel-engineering-blue-black.png "Drexel Engineering")
