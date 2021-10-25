# DHBWorld - Software Requirements Specification 

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
- [Specific Requirements](#3-specific-requirements)
    - [Functionality](#31-functionality)
    - [Usability](#32-usability)
    - [Reliability](#33-reliability)
    - [Performance](#34-performance)
    - [Supportability](#35-supportability)
    - [Design Constraints](#36-design-constraints)
    - [Online User Documentation and Help System Requirements](#37-on-line-user-documentation-and-help-system-requirements)
    - [Purchased Components](#38-purchased-components)
    - [Interfaces](#39-interfaces)
    - [Licensing Requirements](#310-licensing-requirements)
    - [Legal, Copyright And Other Notices](#311-legal-copyright-and-other-notices)
    - [Applicable Standards](#312-applicable-standards)
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
Every project has different roles. As mentioned above added members get the developer role automatically. If you want to change roles you go again to the project settings and and click on "Access". Here you see your team members and their roles.
![alt text](https://i.imgur.com/1Lh8BIL.png "Access sttings")
Over grant role you can give different users or groups a role in your project. If you want to know more about the roles you can go to the administration settings of the youtrack server.
![alt text](https://i.imgur.com/GRIeQTt.png "Server administration settings")
Here you go to Access Management -> Roles.
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

So the last thing is the chart settings. To see the changes you do here just check the Board (Sprint) diagram like [Overview](#21-overview). So now you see the chart and the chart settings. It should look like this:
![alt text](https://i.imgur.com/RpoeRrv.png "Chart and Chart Settings")
Here you can choose the type, the calculation and the issue filter. This is a really minimalistic chart. To get better ones we will create a report in the next big point.

## 3. Specific Requirements

### 3.1 Functionality


#### 3.1.1 Posting a session

#### 3.1.2 Getting an overview


#### 3.1.3 Creating an account

#### 3.1.4 Logging in


#### 3.1.5 Logging out


#### 3.1.6 Joining a session

#### 3.1.7 Keeping track of your sessions

#### 3.1.8 Leaving a session

#### 3.1.9 Finding a session

#### 3.1.10 Getting in touch

#### 3.1.11 Presenting yourself and checking out others

#### 3.1.12 Reporting users and managing friends

#### 3.1.13 Banning users and deleting posts

### 3.2 Usability

#### 3.2.1 No training time needed

#### 3.2.2 Familiar Feeling

### 3.3 Reliability

#### 3.3.1 Availability

#### 3.3.2 Defect Rate

### 3.4 Performance

#### 3.4.1 Capacity

#### 3.4.2 Storage 

#### 3.4.3 App perfomance / Response time

### 3.5 Supportability

#### 3.5.1 Coding Standards

#### 3.5.2 Testing Strategy

### 3.6 Design Constraints

### 3.7 On-line User Documentation and Help System Requirements

### 3.8 Purchased Components

### 3.9 Interfaces

#### 3.9.1 User Interfaces

#### 3.9.2 Hardware Interfaces

#### 3.9.3 Software Interfaces

#### 3.9.4 Communication Interfaces

### 3.10 Licensing Requirements

### 3.11 Legal, Copyright, and Other Notices

### 3.12 Applicable Standards

## 4. Supporting Information
