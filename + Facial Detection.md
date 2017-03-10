# Building Facial Detection Bot Walk Through

## Introduction
For this walk through I will be explaining step by step on how to build the Facial Detection Bot. This walk through was adapted from Sandeep Shekhawat's walk through; a software engineer of Microsoft. What I have done that is different is I have refined each step so that a none technical individual who is interested in learning to build such technology will be capable of doing so. 

You can find Sandeep Shekawat's walk through and more at the following link: 
https://social.technet.microsoft.com/wiki/contents/articles/36442.build-your-first-bot-application-with-microsoft-bot-framework.aspx

The objective of this walk through is to build a bot that will be able to detect three parameters from an image and return a value for each of the designated parameters. The parameters that we will be using for facial detection are Age, Gender, and Smile. The result should look like this:

![botapppic8](https://cloud.githubusercontent.com/assets/25268970/23782196/6a0f1400-0520-11e7-8402-58d1e1df64c2.png)

![botapppic9](https://cloud.githubusercontent.com/assets/25268970/23782447/99ef9bde-0522-11e7-89f3-8767e5dadb49.png)

```markdown
* Note: There are some limitations to this bot.
  1) An image can be too large or too small for the facial detection to work. I have found a 1000px X 1000px 
    image will work. I have yet to identify how small an image can be in order for the detection to not work.
  2) Not all faces can be detected.
  3) The Age parameter accuracy is +/- 10 years.
  4) Gender paramters is inaccurate for some images.
  5) Smile parameter needs a little more work as well, but I believe it does good for the number of 
    variations of a smile.
```

Moreover, however the number of flaws associated with this program; it was still fun to do and amazing to see first hand the back-end of this development.

Before you begin, you can play a demo of the Face API here:
https://www.microsoft.com/cognitive-services/en-us/face-api

## Getting Started
