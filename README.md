# Get-EventsFromEventLogs

Right-click the below link, then "Save link as" to save the latest Launch-GetEventsGUI.ps1 script:

[Download latest version of Launch-GetEventsGUI.ps1 - this branch direct raw link](https://raw.githubusercontent.com/SammyKrosoft/Get-EventsFromEventLogs/master/Launch-GetEventsGUI.ps1)

This repository contains both a script to collect event logs, and a GUI that wraps around the script to make it more visual to understand and set the desired options for the collection of events (such as the number of events to collect per machine, which event log to collect from, etc...).

Also, as a bonus, there is a PowerBI template on which you can load the CSV that comes from the script (or the GUI) to have a visual status about the errors, warnings, etc... or about the events by category, by server...

See the blog post about both the script and the GUI there :

[Get-EventsFromEventLogs.ps1 script](https://blogs.technet.microsoft.com/samdrey/2018/05/04/how-to-use-powerbi-event-log-analysis-template-with-your-own-events-csv-file/ "Use the Get-EventsFromEventLogs.ps1 script to collect the events, and analyze them visually with the provided PowerBI template !")


[Event Collection Graphical User Interface](https://blogs.technet.microsoft.com/samdrey/2018/05/23/event-logs-csv-collector-created-a-graphical-user-interface-around-the-get-eventsfromeventlogs-ps1-script/ "Use the GUI to start the event collection on one or multiple servers, and analyze them visually with the provided PowerBI template !")

Of course, you can still use our good old but still excellent Excel  to create your own graphics and statistical views about the collected CSV events.

## Events collection Script

Just a script to collect events from various sources, including the Crimson Events Channel if you know the name of these, just paste it using -EventLogName property

![Fig1](/Screenshots/GetEventsFromEventLogs-script.png)

## Events collection Graphical User Interface (GUI)

Using Powershell and WPF, I made a GUI to launch the events collection so that the options are easier to view before launching the collection, and you don't have to think about how to spell this or that property, and you see immediately which properties you can use with it...

![Fig2](/Screenshots/GetEventsFromEventLogs-GUI.png)
