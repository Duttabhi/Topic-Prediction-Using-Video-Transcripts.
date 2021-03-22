# Topic Modelling.
Topic modelling of transcript-ed you-tube videos

**Objective:** *Extract the important topics associated with the video by genrating it's transcript and making predictions based on that.*

Detailed report can be found at: https://duttabhi.github.io/Topic-Prediction-Using-Video-Transcripts./report.html

*Following are the details of it.*

Contents
Readings
Requirements
Procedure
Diagram
Working
Conclusion

**1. Readings**

**a. Topic modelling**

It is a process to automatically identify topics present in a text object and to derive hidden patterns exhibited by a text corpus. It assists in better decision making.

**b. LDA(Latent Dirichlet Allocation)**

LDA’s approach to topic modeling is that, it considers each document as a collection of topics in a certain proportion, and each topic as a collection of keywords, again, in a certain proportion.

Once we provide the algorithm with the number of topics, all it does it to rearrange the topics distribution within the documents and keywords distribution within the topics to obtain a good composition of topic-keywords distribution.

**2. Requirements**

python 3.7

jupyter notebook 5.7.4

pafy 0.5.4

ffmpeg 0.1.17

spaCy 2.0.18

nltk 3.4

gensim 3.6.0

google sppech API

**3. Procedure**

Download pafy, tqdm, FFmpeg, spaCy, nltk and gensim. Enable google speech to text API and set its credentials.

import packages

Extract audio from video.

Convert .webm to .wav format.

Break the audio file in smaller audio parts(here, 30 seconds each).

Convert each audio to text and store the transcription in one text file.

Similar process is applied to all the videos.

Get transcription of some videos and combine in one to prepare the data-set.

Remove repetition, similar words, stop words(cleaning) and tokenize it.

Prepare a dicitionary for it and select some best topics out of it(using LDA model).

Provide the transcription to model and slect the topic with more probability.

Assign the most suitable lable.

Check for correctness of topic.
