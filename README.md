# Get-EventsFromEventLogs and analysis with PowerBI

This repository hosts a script to collect event logs (wrapped around Get-WinEvents cmdlet, just made it a bit more intuitive, and created a GUI to make it even more intuitive) as well as a few PowerBI templates to help analyzing the events.

See my older [docs.microsoft.com](https://docs.microsoft.com/en-us/archive/blogs/samdrey/how-to-use-powerbi-event-log-analysis-template-with-your-own-events-csv-file) article to have an idea about how to load your CSV from this script into the PowerBI temlpate.

## Step 1 - Collect the events with the script or the GUI

Right-click the below link, then "Save link as" to save the latest Launch-GetEventsGUI.ps1 script:

> [Download latest version of Launch-GetEventsGUI.ps1 - this branch direct raw link](https://raw.githubusercontent.com/SammyKrosoft/Get-EventsFromEventLogs/master/Launch-GetEventsGUI.ps1)

This repository contains both a script to collect event logs, and a GUI that wraps around the script to make it more visual to understand and set the desired options for the collection of events (such as the number of events to collect per machine, which event log to collect from, etc...).

Also, as a bonus, there is a PowerBI template on which you can load the CSV that comes from the script (or the GUI) to have a visual status about the errors, warnings, etc... or about the events by category, by server...

See the blog post about both the script and the GUI there :

[Get-EventsFromEventLogs.ps1 script](https://blogs.technet.microsoft.com/samdrey/2018/05/04/how-to-use-powerbi-event-log-analysis-template-with-your-own-events-csv-file/ "Use the Get-EventsFromEventLogs.ps1 script to collect the events, and analyze them visually with the provided PowerBI template !")


[Event Collection Graphical User Interface](https://blogs.technet.microsoft.com/samdrey/2018/05/23/event-logs-csv-collector-created-a-graphical-user-interface-around-the-get-eventsfromeventlogs-ps1-script/ "Use the GUI to start the event collection on one or multiple servers, and analyze them visually with the provided PowerBI template !")

Of course, you can still use our good old but still excellent Excel  to create your own graphics and statistical views about the collected CSV events.

### Events collection Script

Just a script to collect events from various sources, including the Crimson Events Channel if you know the name of these, just paste it using -EventLogName property

![Fig1](/Screenshots/GetEventsFromEventLogs-script.png)

### Events collection Graphical User Interface (GUI)

Using Powershell and WPF, I made a GUI to launch the events collection so that the options are easier to view before launching the collection, and you don't have to think about how to spell this or that property, and you see immediately which properties you can use with it...

![Fig2](/Screenshots/GetEventsFromEventLogs-GUI.png)

## Step 2 - Open your CSV in one of the templates

See the link on [docs.microsoft.com](https://docs.microsoft.com/en-us/archive/blogs/samdrey/how-to-use-powerbi-event-log-analysis-template-with-your-own-events-csv-file) for how to open your CSV within a PowerBI template, for now I'll just put a few screenshots to give you an idea of what each template look like.

### Template v1.2.1

![image](https://user-images.githubusercontent.com/33433229/152837324-7edc9fe9-41af-4f21-b5b5-25cce1b9b33c.png)

And the last tab for finer analysis (even research):

![image](https://user-images.githubusercontent.com/33433229/152837419-cc56cc14-8d8f-400e-97c7-2e89b9ef50b4.png)

### Template v1.3

Here I made the first page cleaner than v1.2.x, and changed the orientation of some visuals as it's more readable if you have lots of servers in your CSV:

![image](https://user-images.githubusercontent.com/33433229/152838523-b4a38e64-c7c2-48a6-87e7-be5ab3ee4034.png)

And the last tab for finer analysis is the same as v1.2.1

![image](https://user-images.githubusercontent.com/33433229/152838799-781fbee3-4933-4618-a0e2-0a8069f7c985.png)

### Template v1.4

Introducing a major evolution of the above templates by my awesome, exceptionnal and passionate colleague **Matthys Shoeman** ! :hugs:

![image](https://user-images.githubusercontent.com/33433229/152840511-16de2c74-907f-4702-896a-cf143ea04cf7.png)

there's more:

![image](https://user-images.githubusercontent.com/33433229/152840988-461564b9-8218-495e-9218-cd4164342095.png)

And finally a nice events dashboard:

![image](https://user-images.githubusercontent.com/33433229/152841088-e5f26478-2557-4175-8e34-b6ac4959a9cf.png)

### Template v1.5

Again, by **Matthys Shoeman**, an evolution of the previous template:

![image](https://user-images.githubusercontent.com/33433229/153720055-1afb2de6-9290-46d6-b925-2d9ff0fd8640.png)

And:

![image](https://user-images.githubusercontent.com/33433229/153720070-474d3be7-f473-4211-b464-a8a68859ea26.png)


