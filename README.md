# Invoke-IISLogCleanup
Simple function for clearing IIS logs.



**.SYNOPSIS**

This function is intended to be utilized while cleaning up IIS logs.


**.DESCRIPTION**

This function cleans up log files located within inetpub. It will retain X days worth of logs where X is DaysToKeep.
During the cleanup the process will log the number of log files and the space they consume as well as any that were
deleted.


**.PARAMETER DaysToKeep**

The number of days worth of logs to retain decending from todays date.


**.PARAMETER InetpubLocation**

Location of the inetpub folder for processing


**.PARAMETER LogPath**

Path for script log


**.EXAMPLE**

PS C:\WINDOWS\system32> Invoke-IISLogCleanup -DaysToKeep 7 -Inetpublocation 'D:\Inetpub\logs' -LogPath 'C:\windows\temp';   
