# Youtrack - Beginner Guideline

## Table of contents
- [Table of contents](#table-of-contents)
- [Project](#1-project)
    - [Create a Project](#11-create-a-project)
    - [Team](#12-team)
    - [Roles](#13-roles)
    - [Time Tracking](#14-time-tracking)
    - [Check](#15-check)
- [Agile Board](#2-agile-board)
    - [Overview](#21-overview)
    - [Sprints](#22-sprints)
    - [New Swimlane](#23-new-swimlane)
    - [Cards](#24-cards)
    - [Board Time Tracking](#25-board-time-tracking)
    - [Board Settings](#26-board-settings)
- [Report and Dashboard](#3-report-and-dashboard)
    - [Create a Report](#31-create-a-report)
    - [Dashboard](#32-dashboard)
- [Supporting Information](#4-supporting-information)

## 1. Project

### 1.1 Create a Project
To create a project you go to projects -> create project.
![alt text](https://i.imgur.com/Mew2ZuL.png "Creating a Project")
Now you can name your project, give it an ID, choose the project type and give it a description.

### 1.2 Team
The first important thing to do is to invite people that you want to work with in your project. So to do this you have to go to the project settings. You can find it if you click on your project in the projects tab.
![alt text](https://i.imgur.com/qakeBNC.png "Project Settings")
Now you see the project settings on the right
![alt text](https://i.imgur.com/vlou2oo.png "Project Settings")
Now you click on "Team" and can add new team members over the "Add members" button. You can only add users which are registered to the youtrack server. If you add an user he gets the role developer.

### 1.3 Roles
Every project has different roles. As mentioned above added members get the developer role automatically. If you want to change roles you go again to the project settings and and click on "Access". Here you see your team members and their roles. Over grant role you can give different users or groups a role in your project.
![alt text](https://i.imgur.com/1Lh8BIL.png "Access sttings")
If you want to know more about the roles you can go to the administration settings of the youtrack server. Here you go to Access Management -> Roles.
![alt text](https://i.imgur.com/GRIeQTt.png "Server administration settings")
![alt text](https://i.imgur.com/3NBp5Ai.png "Roles")
Here you see a list of all the roles on the youtrack server and their permissions. If you are the owner of the server you can also add roles to the server.

### 1.4 Time Tracking
So before you can go to the agile board(s) of your project I would recommend that you enable time tracking. It allows you to automatically track the time if a card/task is in progress. So to enable time tracking you go again to the project settings and choose time tracking. Now you set the settings like the following picture:
![alt text](https://i.imgur.com/YekUMSh.png "Time Tracking Settings")
After that you go to workflow (also in the project settings) and click on "Attach workflows". Then you search for the "In Progress Work Timer".
![alt text](https://i.imgur.com/AfvIKTT.png "Workflows - In Progress Work Timer")
If you have never set up this work flow before you will get a "requires setup" notification next to the "In Progress Work Timer". Now click on the "+" right next to the workflow and go to the rules which have this notification. Simply click "configure project" and it will configure it automatically.
![alt text](https://i.imgur.com/DO82CBh.png "Workflow setup")


### 1.5 Check
Now you should have set up your project well enough to actually use the tool now to a certain extent.
Check if you did not have forgotten to set up:
- Your team
- The roles of the team members
- Time Tracking


## 2. Agile Board

### 2.1 Overview
Here you see a quick overview over an agile board
![alt text](https://i.imgur.com/aHf1mlD.png "Agile Board - Overview")

### 2.2 Sprints
So everytime you work in your project you are in a sprint. So sprints are usually a period of time between 1 - 4 weeks. So to create a new sprint you click on the current sprint and click "new sprint".
![alt text](https://i.imgur.com/YAFERbc.png "New Sprint")
Now you can give the sprint a name, a goal and setup a period of time. If you create it, the sprint is automatically chosen and you can start it (if you want) or create every sprint before the project even started.

### 2.3 New Swimlane
If you click on new swimlane in the bottom right of the page you can create a new swimlane (who could have guessed?). So then it opens a window with different settings for the swimlane.
![alt text](https://i.imgur.com/6p3yzWl.png "Swimlane")

I recommend to fill up every red marked setting.
Now you can also see the fields estimation and time spent which would not been there if we did not set up the time tracking settings.
Maybe you noticed that you can only create a swimlane with the type "User Story" I will get to that later in the board settings.

### 2.4 Cards

To create a new card you simply click "new card" in a swimlane and it will create a card in the swimlane.
![alt text](https://i.imgur.com/ZFBOlcs.png "Card")

I recommend to fill up every red marked setting.

### 2.5 Board Time Tracking
So now we can use the time tracking. If you drag and drop a card in the state "In Progress" a timer will start. If you drag and drop it into another column (Open, To Verify, Done) the timer will automatically stop and add the time to the current card.
Now you can click on the card and see the history. Which team member worked at the task for how much time. It even shows you a little circle if you are in the estimation that you have set before or if the task is overdue.
![alt text](https://i.imgur.com/9ldJclf.png "Time Tracking Card")

### 2.6 Board Settings
You can configure some things on your board to do this go to the board settings you can find it in the picture at [Overview](#21-overview). Here you can find general settings which I will not cover here because there is nothing to set up but if you are interested you can give it at quick look. The important settings are at "Columns and Swimlanes" here you can add an extra column if you need it and here we see why we can only create swimlanes with the type "User Story".
![alt text](https://i.imgur.com/48YLJH3.png "Columns and Swimlanes")
If you add a new type then you can also create for example a swimlane with the type Bug, Epic, ...
But is this really necessary? You decide.

So the last thing is the chart settings. To see the changes you do here, just check the Board (Sprint) diagram like [Overview](#21-overview). So now you see the chart and the chart settings. It should look like this:
![alt text](https://i.imgur.com/RpoeRrv.png "Chart and Chart Settings")
Here you can choose the type, the calculation and the issue filter. This is a really minimalistic chart. To get better ones we will create a report in the next big point.

## 3. Report and Dashboard

### 3.1 Create a Report
To create a report simply click on "Reports" and then you see different variations of reports. You can choose which type. So this is an example for a burndown chart.
![alt text](https://i.imgur.com/vmiqygD.png "Burndown")
I think the settings are self explaining. The most important setting is the "Original estimation field". Issue count and Story points make the most sense I think to choose it to show a good report. You can also select "Estimation" but then make sure to set the second "Original estimation field" to Time Spent. Otherwise you can left the seoncd "Original estimation field" empty. So here you see my report from the picture above.
![alt text](https://i.imgur.com/4MvnXu4.png "Burndown example")
So in the top right you can manually recalculate your report and even change the settings. On the y-axis you see the "Original estimation field" and on the x-axis you see the timeline. 


### 3.2 Dashboard
Dash

## 4. Supporting Information
