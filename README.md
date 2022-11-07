# DSCI 511: Data Acquisition and Pre-Processing <br> Term Project Phase 1: Scoping a data set

----------------

# <span style="color:#6666ff">Team Members</span>

- Harsh Bolakani hvb36@drexel.edu
- Greg Morgan gm655@drexel.edu
- Trevor Pawlewicz tmp365@drexel.edu

#### 1. Areas of expertise:
- Harsh: <span style="color:#66ffff">Java, Backend-Development, API-Development, Test Automation, API, Library Design</span>
- Greg: <span style="color:#66ffff">Strengths: Python, AWS Cloud Based Architectures, REST API development, Data Streaming Technologies</span>
- Trev: <span style="color:#66ffff">Front-end UI, Evidence-based User Experience, Design Thinking, Team Leadership</span>

#### 2. Areas to grow:
- Harsh: <span style="color:#00ccff">Data science, AI/ML, Security</span>
- Greg: <span style="color:#00ccff">Growth Areas: Using Python for Data science, Broaden Technical Experience (AI/Machine Learning, UI/UX), Team Leadership</span>
- Trev: <span style="color:#00ccff">Product Management, API building/understanding</span>

----------------

## <span style="color:#6666ff">Our Topic:</span>

We will explore the area of music and lyrical content, possibly notes and chord progressions, to find trends in popular music.
We will ask if popular hit music (chart ranking and top selling songs) have trends in the following way:
- Are there common words and/or phrases?
- Are the common themes?
- Are there common notes and chords?
- Is there a structure in notes/chords that make certain moods?

----------------

> ## <span style="color:#6666ff">Our Phase 1 Report:</span>
>
> ## _a background report on the team's members, their self-identified skills, and individual contributions_
>
> #### 1. Areas of expertise:
> - Harsh: <span style="color:#66ffff">Java, Backend-Development, API-Development, Test Automation, API, Library Design</span>
> - Greg: <span style="color:#66ffff">Strengths: Python, AWS Cloud Based Architectures, REST API development, Data Streaming Technologies</span>
> - Trev: <span style="color:#66ffff">Front-end UI, Evidence-based User Experience, Design Thinking, Team Leadership</span>

> ## _a discussion of what you would like to your data to do/hope it is good for_
>
> 1. Create inspiration for musicians.
> 2. Help musicians over creative road-blocks.
> 3. Assist content producers in creating the perfect song to fit their needs.
> 4. Looking at trends in genres.

> ## _an exhibition of a sample of your data&mdash;show me it exists and what it looks like, even if very raw_
>
> ## __musixmatch__: track.lyrics.get
>   https://developer.musixmatch.com/documentation
>
> ```json
>   "message": {
>       "header": {
>        "status_code": 200,
>        "execute_time": 0.04367995262146
>        },
>        "body": {
>        "lyrics": {
>            "lyrics_id": 7260188,
>           "restricted": 0,
>        "instrumental": 0,
>        "lyrics_body": "Now and then I think of when we were together\r\n...",
>        "lyrics_language": "en",
>       "script_tracking_url": "http:\/\/tracking.musixmatch.com\/t1.0\/m42By\/J7rv9z",
>            "pixel_tracking_url": "http:\/\/tracking.musixmatch.com\/t1.0\/m42By\/J7rv9z6q9he7AA",
>            "lyrics_copyright": "Lyrics powered by www.musiXmatch.com",
>            "backlink_url:" "https://www.musixmatch.com/lyrics/Gotye-feat-Kimbra/Somebody-That-I-Used-to-Know"
>            "updated_time": "2012-04-26T02:09:39Z"
>        }
>        }
>    }
>    }
>```

> ## _a discussion of who might be interested in your data set_
>
> - Musicians
> - Writers
> - Producers
> - Music Industry Professionals
>
> ## _a discussion of how your data is limited and could be improved_
>
> - Free
> - Limited to 2k API Calls daily
> - Free testing plan for evaluation only
> - Access to _ONLY_ 30% of lyrics per song
> - Understanding which part of the song (beginning, middle, end) contains the lyrics that are needed to be best analyzed for our dataset.

> ## _a discussion of how your data were created, e.g., people texting..._
>
> - Musixmatch offer our large-scale lyrics dataset designed to allow machine learning companies and researchers use a wide range of applications like lyrics text analysis which creates music recommendations and provides insights.

> ## _a discussion of what sort of access rights presently exist on your data and how/if you will make them available_
>
> - Register for an _**musixmatch**_ API key:
>
> All you need to do is register in order to get your API key, a mandatory parameter for most of our API calls. It’s your personal identifier and should be kept secret

----------------
> ## <span style="color:#6666ff">Comments for Resubmission:</span>
>
> This is a great project! You have a unique and interesting idea. When it comes to execution, however, it’s unclear how you will be able to answer all four questions laid out in the beginning of the report based on the APIs you listed and the sample data. For example, how will you get the notes and chords data, and how will they be incorporated with lyrics? Is each row of your dataset going to be a line of the lyrics or an entire song? Hammering these down will help you have a better idea of not only what data to collect, but also how large your final data size might be so you can also determine how you need to distribute the data – will you have to distribute access code, or will you be able to directly provide links to stored data.

> ### - discussion of how/if you will make them available – 0/2, how will you make your product available?
> _determine what modes of distribution will be possible once its produces..._
> - finalized outpile file of either JSON or CSV and provide links to stored data

> ### - why you believe it will be possible to conduct - 3/5
> - Several API’s are available for lyric searching
> - Using Web scraping for mining lyric content- Extracting hyperlinks for a crawl

> ### - discussion of the sorts of tasks that will be involved – 3/5, no discussion on tasks
> #### _Tasks:_
> 1) get a list of tracks from musix match.
> 2) acquire the lyrics data for those tracks (either from API or scrapping).
> 3) acquire the mood data for each track.
> 4) for each track count the words.
> 5) assign to the word counts to a mood based on the mood of the track.
> 6) order the words for each mood based on count.
> 7) output finalized dataset to a file.

> ### - how long you believe it will take to build - 3/5, no discussion on timeline
> #### _Timeline:_
> 1) get list of tracks = 3 days
> 2) acquire the lyrics data for those tracks = 3 days
> 3) acquire the mood data = 3 days
> 4) count the words of tracks = 3 days
> 5) assign to the word counts to a moods = 3 days
> 6) order the words = 3 days
> 7) finalize output file = 1 day (1-6 hours)

> ### - abstract – 3/5, no abstract
> #### _summary of your data collection methods_
> - using an API approach for mining
> - also using web scraping as an alternative approach
> - combing both approaches to give a unique journey/product
>
> ```json
> { "sad" : [("cry": 200), ("lose", 150), ("feel", 100)], "happy": [("smile": 243), ("laugh":150)]}
>```

-----
## <span style="color:#ffccff">Notes: More APIs for Lyrics:</span>


1. ### _MusixMatch API_

Musixmatch is a large catalog of song lyrics and translations. The Musixmatch lyrics APITrack this API enables users to legally search for songs by artist, title or lyrics. Get requests return lyrics in JSON or XML formats. The API also provides detailed metadata about the artists who performed it, the genre, influences, related artists and more.

https://www.programmableweb.com/api/musixmatch
