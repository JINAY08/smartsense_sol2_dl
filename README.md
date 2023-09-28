# SmartSense Assessment-2

For this problem statement, I used the librosa library to analyze the given audios (podcasts) and the common Deepgram API for achieving the purpose. 

## Organisation of the Repository:

- The source code for the given problem statement is given in folder ['src\'](./src), wherein you could find the Python notebook that could be run in a single click by clicking on the Google Colab option.
- The data for this problem statement could not be uploaded directly, owing to the large size, but the link has been provided in the ['audio\'](./audio) folder.
- The requirements are specified in the [requirements.txt](requirements.txt) file.
The requirements could be installed using the following command:
```
pip install -r requirements.txt
```

## Approach

I was given three podcast audios, each ranging from around 45 mins-1 hour. So as a first step, to enable summarization and extraction, I would need to convert the audio to text, and then learn the tokenization embeddings. I first learnt the features from the three podcasts, and then trained a Sequential model to know how the training data fits. I could get a training accuracy of nearly 66.67 % after 10 epochs.
Once it was done, I had to convert the audio to text features for analysis. I used the Deepgram API to convert audio to transcript and then smoothened out the transcript by converting them to sensible paragraphs.
And when using the paragraphs, the transcript could be amazingly printed. I also calculated the frequency of the words spoken for the highest time. This could further be used for summarization.

## Results 

Some of the results, including waveforms of the audio, frequency plots, and examples of sentences are being shown below:

\center{
Audio Wave for Podcast-1:

![audio_wave](https://github.com/JINAY08/smartsense_sol2_dl/blob/main/images/audio_wave.png)

A snap from the transcript of Podcast-1:

![para](https://github.com/JINAY08/smartsense_sol2_dl/blob/main/images/para.png)

Frequency Plot showing commonly used words in Podcast-1:

![freq](https://github.com/JINAY08/smartsense_sol2_dl/blob/main/images/freq.png)

}
