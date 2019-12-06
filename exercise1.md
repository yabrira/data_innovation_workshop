# Claiming your workspace and connecting a source
For the live workshop exercises, Segment has pre-provisioned workspaces for the workshop.  If you are doing this workshop after the live event, you will need a new Business Tier workspace with Personas enabled from Segment, or you will need to use your existing Segment workspace. If you do not have one, please contact your Segment sales representative at https://segment.com/contact/sales/.
To get your workshop workspace:
1. Open the Google Sheet at [Segment Workspaces](https://docs.google.com/spreadsheets/d/17FvUoABdw2bA_cRhEqaJ6j3P3VoCm4pIfq7RfvScvRc/edit?usp=sharing)
2. Find an unclaimed workspace
![](https://paper.dropbox.com/ep/redirect/image?url=https%3A%2F%2Fpaper-attachments.dropbox.com%2Fs_4F971EE2E8698F2EB68A6C5183D3804CDEC6E0DE0A589AB3E5D2C1E561F6F6AB_1575658462808_Screen%2BShot%2B2019-12-06%2Bat%2B6.42.44%2BPM.png&hmac=TBzY87FZQs4OgDl9g3Cq6DPELwdBZ0WRYTkd64RWPlg%3D)
3. Claim your shiny new Segment workspace by putting your name in the appropriate fields, please.
## Part 1 - Set up Your Segment Workspace
After you have claimed your workspace, there are a couple of steps you need to follow to get it ready to start the workshop.
1. Go to [https://app.segment.com](https://app.segment.com/).
2. Make sure you select the “Password” login radio button.
3. Log in as:
```
username: yanis.b+apidays_workshop_paris@segment.com
password: <will be on the whiteboard>
```
![](https://paper-attachments.dropbox.com/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1558297663348_image.png)
4. Click the “Log In” button.
5. Find the workspace name you claimed in the spreadsheet.
6. Click the tile with the name you claimed.
![](https://paper-attachments.dropbox.com/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1558298143343_image.png)
7. Click on the Settings gear in the bottom left corner of the screen that appears.
![](https://paper-attachments.dropbox.com/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1558298296954_image.png)
8. Change the name of the workspace to something you will remember, so that you can find your workspace more easily in case you have to log back in during or after the workshop.
9. Add `igor+awsmlworkshop@segment.com` in the Incident Contact section.
10. Click the “Save Changes” button.
![](https://paper-attachments.dropbox.com/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1558298453353_image.png)
## Part 2 - Create Segment Sources
Segment Sources allow you to collect semantic events as your users interact with your web sites, mobile applications, or server-side applications.  For this workshop, you will set up sources for a web application, an Android application, and iOS mobile application.  We will also create a source that will be used to send recommendations from Personalize to user profiles in Segment.
Your initial Segment workspace will look like this:
![](https://d2mxuefqeaa7sj.cloudfront.net/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1551126460468_image.png)
You will need to add four sources, using the ‘Add Source’ button in the screen shot above.  To set up a source:
![](https://d2mxuefqeaa7sj.cloudfront.net/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1551126918810_image.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1551126938657_image.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1551126965261_image.png)
![](https://d2mxuefqeaa7sj.cloudfront.net/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1551127036032_image.png)
Once your source is configured, it will appear in your workspace like this:
![](https://d2mxuefqeaa7sj.cloudfront.net/s_539A927F5DA788B557CE05EF51E8221F1D7D02D016B6CA298FD5F55304B8CA28_1551127061361_image.png)
You will need to repeat these steps to configure three more sources.  One for Android, one for iOS, and one for your Personalize events.  
Name your sources as follows:
| Source Name | Source Type | Description |
| ----------- | ----------- | ----------- |
| website-prod | Javascript | Accepts user events from a web site; created in the example above. |
| android-prod | Android | Accepts user events from an Android application. |
| ios-prod | iOS | Accepts user events from an iOS application. |
| personas-event-source | Python | Accepts events from the Personalize service Lambda you will connect in the last exercise. |
For the web source, use the Javascript source type, for Android the Android source, for iOS the iOS source, and for the personas-events-source use the Python source type.
