# Preparation

### *If you are following this workshop outside of the live webinar and do not have a Segment workspace feel free to create it [here](https://segment.com/signup)!*


## Part 1 - Set up Your Segment Workspace

*If you have already created a workspace please bear with us until Part 2.*

Please visit https://segment.com/signup and follow the instructions in order to create a new workspace. 


## Part 2 - Create Segment Source
Segment Sources allow you to collect semantic events as your users interact with your web sites, mobile applications, or server-side applications. For this workshop, you will set up an HTTP source!  
Your initial Segment workspace will look like this:
![](misc/img/workspace_overview.png)  
You will need to add an HTTP source, using the ‘Add Source’ button in the screen shot above. To set up a source:

![](misc/img/http.png)  

![](misc/img/connect.png)  

Please enter "workshop_source" as the source name. It'll be used as part of the request URLs we will be making in exercise 2.
![](misc/img/workshop_name.png)  

Once your source is configured, it will appear in your workspace like this:
![](misc/img/source_done.png)  

## Part 3 - Create a Google analytics instance

As a desination we will be using Google Analytics. If you do not have a GA account to use please go 

1. Create or sign in to your Analytics account:
...Go to google.com/analytics
...Do one of the following:
......To create an account, click Start for free.
......To sign in to your account, Click Sign in to Analytics.

2. [Set up a property in your Analytics account](https://support.google.com/analytics/answer/1042508). A property represents your website or app, and is the collection point in Analytics for the data from your site or app. In our case we need a "Web" property.


## [>>> onwards to exercise 1](exercise1.md/)