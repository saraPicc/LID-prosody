# Language identification based on prosodic features


---

## Theoretical background
<br/>

Prosody is the branch linguistic concerning the suprasegmental features of human speech. Some of these are speech rate, intonation and rythm and they play a fundamental role in the communication act. Prosodic analysis in the frame of a particular language shows that a certain message conveys different shades of meaning due to the variations of these attributes and gives us an idea on how pragmatic meaning is acoustically represented during speech (Leone, Maturi, 2006). 
<br/>
The acoustic features through which prosody can be tracked are:
<br/>
<br/>
*   **Pitch**: it represents the rate of vibration of the vocal folds over time (frequency) and it's expressed in Hz.  It is different for each speaker since it depends on the physical conformation of the vocal tract, gender and age and its variation shapes the intonation in speech utterances.
<br/>

*   **Intensity**: it's the amount of energy (amplitude) over time and is expressed in dB. Peaks of intensity represent emphasis on a certain element.
<br/>

If the analysis of speech rythm shifts to a cross-linguistic perspective, there are different kind of rythm patterns that divide languages in three main groups:


1. Syllable-timed languages: the rythm is marked on syllables (Italian, Spanish, Finnish)

2. Stress-timed languages: the rythm is marked on stressed syllables (German, English, Dutch)

3. Mora-timed languages: rythm is marked on mora (Japanese)


These differences depend on phonologic, phonetic, lexical and synctatic facts. On a phonetic level, the patterns of rythm vary due to speech rate and tempo variation, so langauges that are classified as syllable-timed can tend to a stress-timed rythm in some situation and, on the other hand, stresst-timed languages can have a  syllable-timed language rythm (Auer, 2001).

<br/>
<br/>

## Aim of the project

The aim of this project is to train a Neural Network to create a language classifier based on audio data. The features used for the classification consist intensity and pitch, acoustic features that represent prosody in human speech.
The languages involved in the project are Italian and German.
During the project the sampling rate of the data is manipulated to create experimental sets and see how the learning of the model differs by changing the amount of information used as an input. Also, different kinds of binning and two kinds of matrices (2D and 3D) are used as experimental paramenters.  

<br/>

## Data

The audio files for the training, test and validation have been taken from Common Voice. This is a project of the Mozilla Foundation consisting in an open-source audio dataset involving more than 80 languages. The audio clips are read sentences generated and reviewed by volunteer contributors, speakers of different gender and age. Speaker's accent is also tracked in the corpus. 
Each audio file is well documented with demographic metadata, the read text and the information of the audio including path to the downloaded audio file, the decoded audio array, and the sampling rate.

I think this is a good corpus to work on this taks because it's inclusive with respect to speaker gender, age and accents and since data consists in read sentences of length ranging from approximately 2 to 20 seconds the prosodic patterns are somehow homogeneous and the stress typology of the languages involved is preserved, helping the classification.

<br/>

## Problems and challenges

A problem is represented by the limited amount of data availale for certain languages (for example, there are ~20 hours of italian data). A consequence of the limited amount of data is that a balance between speakers that belong to different gender and age might be lacking. 
Another limitation is represented by the use of Google Colab, that in its free version provides GPU usage but the runtimes are limited to 12 hours and the RAM is limited to 16 GB. Managing such a big quantity of audio data has sometimes caused session crashes. 

