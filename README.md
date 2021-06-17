# VODClassifier

## What is this?
The VODClassifier is an offshoot program of the [TwitchClipAnalyzer](https://github.com/KilometersFan/TwitchClipAnalyzer) designed to take in data generated by the TCA and train a ML model to predict the sentiment (category) of Twitch Chat throughout a broadcast.

## About the Data
The training data is based on the emotes Twitch Chat uses during a broadcast. The chat is processed to find groups of comments that have high emote usage, which are then processed to see which of the user-defined categories best fit each group. It was often found during testing that the data was highly imbalanced, so in the TCA repo, there is an [Upsampler](https://github.com/KilometersFan/TwitchClipAnalyzer/blob/epic/2021-refactor/ClipBot/Upsampler.py) file that will upsample the minority classes. All of the text processing is done in the TCA, so for more information please visit the that repository.
