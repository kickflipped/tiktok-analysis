# What the Rise of Tik Tok Could Mean for Spotify & the Future of Music Streaming: An First Look

Watching TikTok become wildly popular these past few year and with Spotify being one of the most popular streaming services, it led me to wonder how exactly Tik Tok has affected music streaming and artist and song popularity. Does this platform really have a noticeable impact on popular music, or are these cases rare? I decided to perform an exploratory data analysis to help visualize and better understand the correlation between what songs are promoted on the Tik Tok algorithm and what is popular on Spotify.

# Project Goals

The main questions I want to answer: 
- Does TikTok have a significant influence on what songs become popular on Spotify?

- If there is a correlation or relationship between “tik tok famous” songs and songs on the top charts, how has it changed as the app continues to grow? 

- And finally, how could this new social media platform change things for Spotify? 

# Data Analysis, Initial Thoughts, and Summary of Process

I used the Spotify API, pandas, matplotlib, and the spotipy libraries to generate my data. A Spotify search led me to playlists of [songs viral on Tik Tok in 2020](https://open.spotify.com/playlist/65LdqYCLcsV0lJoxpeQ6fW?si=iSU447kiTCuQUz-rYz7Dzw), and [songs viral on Tik Tok in 2018](https://open.spotify.com/playlist/73Q2uot60f3KH9N3YolDfV?si=U1Wth-l5QR--fZoyBSteSA). I chose the playlists with the most followers as an indicator of an accurate playlist. I did the same to find the top songs overall for 2020 and 2018. To have data sets of equal sizes, I had to manually merge two “top songs of the year” playlists to get similar sample sizes.

After creating my dataframes, I generated histograms to compare distributions for audio features for Top Tik Tok songs against that of Top Overall songs. The orange histograms are for the Overall Top Songs of the year, and blue for Tik Tok songs. 

My overall observations: 
- For the year 2020, with the exception of song length and tempo, the distributions for each audio feature seems to have very tight overlaps. The types of sounds, features, and thus songs that seem to be popular in one data set correlate well with the other. 
- Tempo having a higher frequency in the Tik Tok data set might be influenced by the larger sample (160 vs 139).
- Song length is interesting: songs popular on Tik Tok seem to be noticeably shorter than the charts. This could be due to the fast-viral-and-short video type content that is the core of Tik Tok. The types of songs that tend to be longer may not have the viral qualities that are often needed to blow up on the app.
- For the year 2018, we see much more variance between distributions, particularly for energy, loudness, valence, and length. Songs on Tik Tok have a greater range in energy, greater range in loudness, slightly higher valence and slightly shorter length. The types of sounds popular on Tik Tok are thus less tightly correlated with the top charts.

![2020 Distribution Graphs](https://github.com/kickflipped/tiktok-analysis/blob/main/Figures/2020.png)
![2018 Distribution Graphs](https://github.com/kickflipped/tiktok-analysis/blob/main/Figures/2018.png)

Then, I generated bar plots to visualize how the similarities of features between what’s popular on Tik Tok versus the charts has changed between 2018 and 2020. (Separated into 2 graphs for visualization purposes, values of similar scale grouped together).

For 11 out of the 12 audio features, the differences in mean for features of Tik Tok songs and Top Chart songs were smaller in 2020 than in 2018. This provides more evidence to support the idea that sounds and songs that are popular on Tik Tok are more highly correlated with overall top songs in 2020. 

![Difference in Means 2018 and 2020 Part A](https://github.com/kickflipped/tiktok-analysis/blob/main/Figures/diffA.png)
![Difference in Means 2018 and 2020 Part B](https://github.com/kickflipped/tiktok-analysis/blob/main/Figures/diffB.png)

# Conclusions and Ideas for the Future

My EDA illustrates that as Tik Tok has grown, the songs popular on the app and songs on the charts become more and more predictive of each other. There’s a high correlation between what gets popular on the app and what is popular overall, and this is especially clear once you look into those playlists and see many, many overaps in songs. Perhaps popular songs find their way onto Tik Tok, which creates yet another avenue for these songs to gain more attention to millions of listeners. On the other hand, songs on Tik Tok might be creating a path for new music to blow up on Spotify: perhaps users are not just passively listening to snippets of songs that blow up, they are making a conscious choice to head over to Spotify and listen to the track. 

But, as an extension to this project, I want to investigate this further and discover whether or not there’s temporal precedence to establish the direction of correlation. Having access to data of when song snippets were added to Tik Tok, and seeing how streams increased after this date differ from the general trajectory of streams before the sound was added, would help establish the direction of the correlation.

Regardless, Tik Tok has a remarkable ability to influence popular music, and popularize chart topping songs even more, by offering such a global, easily shared platform. 

I think Tik Tok can work really well with Spotify’s own marketing strategies and what makes Spotify so loved. Spotify’s own initial launch started with “word-of-mouth” marketing, starting as an “invite-only” service, with existing users having only 5 invites to friends, and now thrives partly off sharing music and playlists all around.

A persistent trend on Tik Tok has people sharing song recommendations and linking their playlists in the comments. Spotify can embrace this digital word of mouth strategy by starting a social media presence on Tik Tok in the same way it and other companies are on other platforms like Twitter. (The official Spotify account only has 1 video!) On Tik Tok, Spotify could curate and show song recommendations with artists it partners with in short Tik Tok videos, which could potentially bring Tik Tok users to Spotify to check these songs out and increase # users and streams. I would describe this as the visual/video version of Spotify’s curated playlists.

I love what music streaming and discovery has done for me as an avid music fan. I’m super passionate about always finding and sharing music with more people, and Tik Tok has the power to help us do just that.






