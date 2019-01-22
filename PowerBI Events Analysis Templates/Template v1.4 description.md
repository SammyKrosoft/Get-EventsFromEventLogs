# An new PowerBI template for Event Log analysis from the great Matthys Schoeman, Senior PFE at Microsoft !

+	Updated the framework view of each tab
-	I have expanded the “Event Types – Count per Log Set (Event Log Collection Info)” landscape to accommodate more Event Log Names for collection
>	The reason for that was, if we can say maybe accommodate any Event Log based on any technology running on the windows operating system, we can list the Event Log Name in this view
>	If we use for example AD guys that does a investigation of SMB 1 connections to DCs on the “Microsoft -Windows-SMBServer/Audit” Event Log Name, then we can list the Event Log name in the overview
>	For this I made use of your normal powershell command called“Get-EventsFromEventLogs.ps1” without the GUI to add the this Event Log in the array. I did not had the time to investigate the GUI version to see how I can add the additional Event Log name in the gui….sorry my powershell is very limited.
>	One thing I tried is to add all the list of Event Log names of a DC or Exchange server – That was a huge fail – it bomb
>	This SMB1 Events is informational and thus the information shows in the overview

[Matt pic 1](./img/Matt_01.png)

+ I added a “Informational only for each server” to accommodate if someone is interested on informational data

[Matt pic 2](./img/Matt_02.png)

-	I added a “Information” part to the “Errors/Warning per Provider” tab and also include filters buttons (in Black) so that you can interact with the data
for each server” to accommodate if someone is interested on informational data

[Matt pic 3](./img/Matt_03.png)

*	I added a “Information” part to the “Detailed Analysis” tab and also include filters buttons (in Black) for the Level Display and Event Source, so that you can interact with the data

[Matt pic 4](./img/Matt_04.png)

+	I added a “Event ID Dashboard” Tab and also include filters buttons (in Black) for the Level Display and Event IDs, so that you can interact with the data

 [Matt pic 5](./img/Matt_05.png)
