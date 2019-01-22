•	Updated the framework view of each tab
•	I have expanded the “Event Types – Count per Log Set (Event Log Collection Info)” landscape to accommodate more Event Log Names for collection
o	The reason for that was, if we can say maybe accommodate any Event Log based on any technology running on the windows operating system, we can list the Event Log Name in this view
	If we use for example AD guys that does a investigation of SMB 1 connections to DCs on the “Microsoft -Windows-SMBServer/Audit” Event Log Name, then we can list the Event Log name in the overview
•	For this I made use of your normal powershell command called“Get-EventsFromEventLogs.ps1” without the GUI to add the this Event Log in the array. I did not had the time to investigate the GUI version to see how I can add the additional Event Log name in the gui….sorry my powershell is very limited.
o	One thing I tried (in my little knowledge of powershell, I tried to add all the list of Event Log names of a DC or Exchange server – That was a huge fail – it bomb) 
•	This SMB1 Events is informational and thus the information shows in the overview

 

•	I added a “Informational only for each server” to accommodate if someone is interested on informational data

 

•	I added a “Information” part to the “Errors/Warning per Provider” tab and also include filters buttons (in Black) so that you can interact with the data
for each server” to accommodate if someone is interested on informational data

 

•	I added a “Information” part to the “Detailed Analysis” tab and also include filters buttons (in Black) for the Level Display and Event Source, so that you can interact with the data
 

•	I added a “Event ID Dashboard” Tab and also include filters buttons (in Black) for the Level Display and Event IDs, so that you can interact with the data

 
