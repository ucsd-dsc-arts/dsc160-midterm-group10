# Project Title

DSC160 Data Science and the Arts - Midterm Project Repository - Spring 2020

Project Team Members: 
- Adam Kreitzman, akreitzm@ucsd.edu
- Jonathan Song Zhang, name2@ucsd.edu
- Joseph Fallon, name3@ucsd.edu
- Ka Ming Chan, kmc026@ucsd.edu
- Yijian Zong, name5@ucsd.edu

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
  Our results will basically just come 

## Data

(10 points) 

This section will describe your data and its origins. Each item should contain a name of the data source, a link to the source, and any necessary background information such as:
- What is your cultural data source? 
- When was it made? 
- Who created the works? 
- Is it digital native, or is it some kind of scan, recording, photo, etc., of an analog form? 

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

- image files (`.jpg`, `.png` or whatever else is appropriate)
- audio files (`.wav`, `.mp3`)
- written text as `.pdf`

## Discussion

(30 points, three to five paragraphs)

The first paragraph should be a short summary describing your results.

The subsequent paragraphs could address questions including:
- Why is this culturally relevant?
- How does your computational approach differ from the traditional art historical, musicological, manuel/subjective approach to analyzing your cultural subject? 
- How do you think the original artists/musicians would respond to this type of analysis? Would it change/inform their practice in some way?
- How do your results relate to broader social, cultural, economic political, etc., issues? 
- In what future directions could you expand this work?

## Team Roles

We were able to effectively distribute the work between team members by having each person be responsible for one artist for each genre as follows:
Adam Kreitzman - Kendrick Lamar and Justin Bieber
Jon Zhang - Chance the Rapper and Katy Pery
Yijian Kong - 
Ka Ming -
Joseph Fallon - 

## Technical Notes and Dependencies

Any implementation details or notes we need to repeat your work. 
- Additional libraries you are using for this project
- Does this code require other pip packages, software, etc?
- Does this code need to run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

References to any papers, techniques, repositories you used:
- Papers
- Repositories
- Blog posts
