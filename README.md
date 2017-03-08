# Smart-Bot-Project
## Introduction

## Walkthrough
Download the open source bot builder SDK
```markdown
https://dev.botframework.com/ 
```
Getting Started
``` markdown
Follow the instructions from the provided link or follow my instructions. Note that my instructions are for 
the people that are newer and require a little more guidance.

https://docs.botframework.com/en-us/csharp/builder/sdkreference/gettingstarted.html

Instructions:
1) Install Visual Studio 2017 from www.visualstudio.com
2) Download and Install Bot Application template from http://aka.ms/bf-bc-vstemplate

* Note: Once the Bot Application zip file is downloaded, be sure to move it to the Visual Studio 2017 
  template directory
  
\...\Documents\Visual Studio 2017\Templates\ProjectTemplates\Visual C#\

3) Open Visual Studio 2017, select File > New > Projects > Visual C# > Bot Application

* Note: Don't worry if you see only 1 Bot Application template

4) Name your first Bot and select OK
```
![botapppic0](https://cloud.githubusercontent.com/assets/25268970/23716194/4e597436-03fd-11e7-9117-0353362e6ed9.png)

```markdown
5) A new window will appear, look to the right hand side and locate the Controllers folder. Click the arrow 
  next to the folder to expand the folder. Double click on MessageContrller.cs to open it in a new tab. 

6) Next, locate Web.config and double click it to open it in another new tab.
```
![botapppic1](https://cloud.githubusercontent.com/assets/25268970/23715743/a670f2fe-03fb-11e7-983a-254a44fb971f.png)
```markdown
MessagesController.cs
```
![botapppic2](https://cloud.githubusercontent.com/assets/25268970/23719750/968403b8-040a-11e7-99e0-5557f629d6ae.png)

```markdown
The MessagesController.cs is the core functionality of the Bot Template. In this case the code takes the 
message text for the user, then creates a reply message using the CreateReplyMessage function. You can 
modify this template to add more functions.
```
```markdown
Web.config
```
![botapppic3](https://cloud.githubusercontent.com/assets/25268970/23720193/0b416cbc-040c-11e7-9e9a-4d9d5d0d4bb6.png)

```markdown
* Note the highlighted.
The bot has to be registered with Bot Connector
The AppId and AppPassword from the Bot Framework registration page have to be recorded in the project's web.config
The project needs to be published to the web
```
