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
> Musixmatch
![Musixmatch logo](images/Monogram_Primary.png "Musixmatch" =100x100)
Genius ![Genius logo](images/Genius.png "Genius" =100x100)

---
#### Building the Dataset:
> 1. Register for an API key (musixmatch)
> 2. Setup Imports and API Authentication (musixmatch)
> 3. Retrieve song list from URL with parameters for a data query (genius)
> 4. Scrape Lyric Data with Beautiful Soup (genius)
> 5. Collect and Merge Data
> 6. Process Data
> 7. Remove Stop Words
> 8. Output the Dataset

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
> ...TBD...

---
#### Discussion of Access Rights:
> ...TBD...

---
#### Issues and Limitations:
> #####_Musixmatch_:
> - Free
> - Limited to 2k API Calls daily
> - Free testing plan for evaluation only
> - Access to ONLY 30% of lyrics per song
> - Understanding which part of the song (beginning, > middle, end) contains the lyrics that are needed to be > best analyzed for our dataset.
>
> Genius.com was web scrapped to get full lyrical content > of songs as a solution to only having access to the > __musixmatch__ free 30% of lyrics per song.
>

---

![Drexel logo](images/Drexel-engineering-blue-black.png "Drexel Engineering")
