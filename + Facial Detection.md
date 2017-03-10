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
```markdown
* Note: Please first build out the Bot Application Template. You can find a walk through of this build in my Smart-Bot-Project repository titled Bot template.md. 
```
1) To begin, you will first need the Cognitive Service Face API (CSF API)
```markdown 
  This API will allow you to show the face attributes such as Age, Gender and Smile from an image that is 
  loaded into your bot  application.

  To get the CSF API, go to the following link:
  https://www.microsoft.com/cognitive-services/en-us/face-api
  
  Create an account; under Free Trial you can find the Face-Preview API and register for it.
  ```  
  2) You will then be taken back to your original portal and you will see the product that you registered for.
  ```markdown
* Note: You do not need to Buy On Azure. Just copy your first key and you will paste this key in the 
  Web.config of your template.
  ```
  3) Open the Web.config file on the right-hand side in your Solution Explorer by double clicking. When the Web.config tab appears, locate the section that has the following information: 
```markdown      
    <add key="BotId" value="" />
    <add key="MicrosoftAppId" value="" />
    <add key="MicrosoftAppPassword" value="" />
```  
  4) Add the following line at the end and paste your key where it says 'paste key here':
```markdown    
    <add key ="FaceAPIKey" value="paste key here">
```    
  5) Save and then navigate to the tool bar at the top of Microsoft Visual Studio and select Project > Manage NuGet Packages.
  
  6) A new tab will appear labeled NuGet: Project Name. Select Browse and type in Microsoft.ProjectOxford.Face in the Search Field. Then
install the package.
```markdown
* Note: This package will automatically be added to your packages.config
```
![botapppic10](https://cloud.githubusercontent.com/assets/25268970/23783410/629b1c56-0529-11e7-9dde-a7729c318419.png)

  7)
