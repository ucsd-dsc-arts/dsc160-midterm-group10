# Project Title

DSC160 Data Science and the Arts - Midterm Project Repository - Spring 2020

Project Team Members: 
- Adam Kreitzman, akreitzm@ucsd.edu
- Jonathan Song Zhang, name2@ucsd.edu
- Joseph Fallon, name3@ucsd.edu
- Ka Ming Chan, kmc026@ucsd.edu
- Yijian Zong, yizong@ucsd.edu

## Abstract

(10 points) 

For the project proposal, please write a short abstact addressing the questions below. You should replace the entire contents of this section with one to two paragraphs addressing the following:

- What is the data set that you are going to analyze?
- What is your research question? 
- What is your hypothesis about the results? 
- What features of the data will you use to address your question? 
- What techniques and software tools will you use to extract these features?
- What analytic techniques will you use?
- What forms will your results take? (graphs, charts, images, sonification, Wordles, etc)
- How are you expanding on topics we have covered in class? 
- Why is it interesting? (personally, culturally, politically, other)

  The dataset that we chose to analyze was 2-3 songs from 10 different artists, 5 of which were pop artists and 5 of which were hip hop artists. We used the website MP3Quack to download the mp3 files compatible with the Librosa library in Python3. The main research question that we were trying to analyze is whether any patterns emerged based on our perceived simplicity of many pop songs in comparison to hip hop songs. We wanted to first see based on the waveplots and spectrograms of the songs of each artist if they were similar in frame and the artists themselves exhibited a particular sound. 
  The features of data that we used were the waveplots and spectrograms of the audio files in order to visualize each song, and then the SVC classifier based on the MFCC's of each song. Our hypothesis about the results is that the songs by the pop artists will exhibit a very formulaic graph whereas the hip hop songs will be much choppy and disorderly simply due to the nature of each genre of music. 
  The techniques we will use rely on the the Librosa library and Sci-Kit Learn libraries in Python3, where we will extract and visualize the waveplots and spectrograms, and then run classification models against the different combinations of songs from each artist to see how easily the model can differentiate between them, as a method of determining the similarity of them. This is definitely not foolproof, but we think it can give us some interesting data.
  Our results will basically just come as the graphs and model accuracy of the different songs. In order to effectively break it up between 5 different people, we are treating it as 5 different test cases and comparing across each one.

## Data

(10 points) 

This section will describe your data and its origins. Each item should contain a name of the data source, a link to the source, and any necessary background information such as:
- What is your cultural data source? 
- When was it made? 
- Who created the works? 
- Is it digital native, or is it some kind of scan, recording, photo, etc., of an analog form? 

  Our cultural dataset it 2-3 songs from 10 different artists, with 5 pop artists and 5 hip hop artists. In a sense, it a dataset of randomized artists from two different genres we created. The songs were all created at different times in the 21st century or the tail end of the 90s, but come from rather recent but established artists. The artists we chose for hip hop were Kendrick Lamar, Chance the Rapper, J Cole, Biggie Smalls, and Future. The artists we chose for pop were Justin Bieber, Katy Perry, Rihanna, Taylor Swift, and Lady Gaga. The data is in the form of mp3 files, which are recordings of their music.

## Code

(20 points)

This section will link to the various code for your project (stored within this repository). Your code should be executable on datahub, should we choose to replicate your result. This includes code for: 

- data acquisition/scraping
- cleaning
- analysis
- generating results. 

Link each of your notebooks or .py files within this section, and provide a brief explanation of what the code does. Reading this section we should have a sense of how to run your code.

## Results

(30 points) 

This section will contain links to documentation of your results. This can include figures, sound files, videos, bitmaps, as appropriate to your domain of analysis. Each result should include a brief textual description, and all should be listed below: 

Because our results were confined to the different case studies and most of our code was directly creating results, the easiest way to follow is by looking at each case study through the pdfs we uploaded to the results section.

## Discussion

(30 points, three to five paragraphs)

(Quick note, for more insight to the specific case studies, check the python notebook containing each, as they go into more depth than we can here for each case study as we are discussing the whole results in this section).

In broad terms, we learned that the songs from pop artists tended to be much formulaic in nature, but that didn't necessarily mean that the SVC model hard a harder time differentiating between the songs, though that was likely the impact of unforeseen factors in our analysis. Because the pop songs were more formulaic, it likely meant that the classifier had a much easier job differentiating between each one. With how arrythmic and unique each hip hop song can be, it makes sense that the classifier could struggle when only presented with a 10 second portion of the song, though this wasn't necessarily something we foresaw happening. However, this was not always the case, as the model had a higher score when run with two J Cole songs being inputted then when run with two Rihanna songs being inputted, while in a different case study, the model run on several combinations of Justin Bieber songs had much higher accuracy than when it was run on different combinations of Kendrick Lamar songs. This shows that these results may be less indicative of the genre of the artist and possibly more correlated to the style of each specific artist as well. With how hip hop music has garnered much more mainstream appeal, it isn't all that surprising to see that certain hip hop artists may have pop qualities to their music, with many songs being a combination of the two genres. One example of that would be future, whose waveplots looked very similar to some of the songs by pop artists rather than other hip hop artists, and had similar results as the songs by Lady Gaga in that specific case study. This could be a manifestation of the fact that Future is among the new style of "mumble rappers" who have received criticism for having music devoid of much lyricism and more focused on beats, with lyricism having long been a staple of the hip hop genre. Perhaps the most interesting case study would come between Taylor Swift and Biggie Smalls, given that Biggie Smalls is the only artist we chose that truly represents old school hip hop before it was mainstream. The waveplots for Biggie were fairly unique to him and fairly different, with high classifier scores, showing a potential shift in hip hop music occurring since the time when Biggie, 2Pac and Nas were the faces of hip hop music to now. For Swift, her patterns weren't very different from the other pop artists, showing our theory of pop music being formulaic to be relatively true. The last case study between Chance the Rapper and Katy Perry generally showed what we expected and had similar results to above.

  We believe that this question is culturally relevant because the simplicity of popular music has been a long debated topic by those who are heavily invested in music. Personally, I remember hearing the disdain of my jazz instructor at what popular music has become because it literally relies on a progression of 4 chords and a catchy chorus, or watching a comedic band called Axis of Awesome playing one chord progression and switching seemlessly between almost 50 different mainstream pop songs. We were curious if we could see if this was true mathematically, and while we didn't necessarily get a clear cut answer from our data, we definitely got some interesting angles to look at it and some preliminary data that suggests this very much could be the case. 
  
  Our computational approach is different than the musicological approach because we are looking at specific sound patterns to try and see whether or not patterns emerge, rather than simply using the ear test the way most people do. In a way, we are applying a mathematical approach to try and see if a lot of the subjective criticisms toward specific artists is valid. I seriously doubt that artists would listen to this because at the end of the day those who produce mainstream music are probably in it more for the money and the fame than those who have more personal reasons for being an artist. I think that a lot of people probably don't care that much about the intracacies that are present in music and want something that is simply easy to listen to.
  
  Another lens in which this could be seen from a broader social and cultural issue is the evolution of hip hop music since it was pioneered by artists like those from N.W.A., or Biggie, 2Pac and many others. Obviously this is very speculative due to our lower sample size, but this is definitely something we might explore if we were to keep researching this. Many critics of current hip hop allege that new artists have utilized the framework built up by artists coming from unprivileged backgrounds and rapping about social injustice to create a new style with mainstream appeal that doesn't do this at all. This could partially be why the work of Kendrick Lamar, who is touted for both his lyricism and growing up in Compton, similar to the rappers in N.W.A., has a much more erratic and unique pattern to his songs when compared to other hip hop artists and pop artists. Obviously, our analysis falls far short to confirm this speculation, but it is something that could allow us to go above an beyond what we did and carry our analysis even further. This criticism hasn't just been by fans of the music industry but by artists as well. It can be seen in songs such as Homicide by Logic and Eminem, where Logic says "Nowadays, everybody sound the same, shit's lame." I think our analysis is very interesting from this specific angle, but as we said before, it isn't necessarily an indication that this is true, but shows that we should dig deeper by using sentiment analysis, and other musical features like chord progression and bag of words to see trends in each artist specific to hip hop artists.
 

## Team Roles

We were able to effectively distribute the work between team members by having each person be responsible for one artist for each genre as follows:
Adam Kreitzman - Kendrick Lamar and Justin Bieber
Jon Zhang - Chance the Rapper and Katy Perry
Yijian Kong - Biggie Smalls and Taylor Swift
Ka Ming - Rihanna and J Cole
Joseph Fallon - Lady Gaga and Future

Adam handled most of the writing duties, but with the help and suggestions of the whole group each step of the way, so we feel as though the project is a good reflection of every individual equally contributing.

## Technical Notes and Dependencies

Any implementation details or notes we need to repeat your work. 
- Additional libraries you are using for this project
- Does this code require other pip packages, software, etc?
- Does this code need to run on some other (non-datahub) platform? (CoLab, etc.)

This project should not be too difficult to replicate, but make sure that the file structure is correct so that Librosa is able to upload the audio files accordingly (in the data folder).

## Reference

References to any papers, techniques, repositories you used:
- Papers
- Repositories
- Blog posts
