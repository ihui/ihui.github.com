---
layout: post
title: "Sync your Google Earth data"
date: 2014-04-28 08:54
comments: true
categories: GIS
---
Do you work lot with Google earth in different computers? and need to tranfer your data such as palcemarkers or lines or area from one to another with USB key? I think you like me want Google Earth to sync them automatically for us. But it does not.  
  
Some guys use cloud services to backup their Google earth data, and fetch data from cloud  on different computers. It's seem like not a bad solution. There is another [clever method](http://productforums.google.com/forum/#!topic/earth/gaH1BgwirJk) which use hard link between directory.  
  
Here are steps what he follow:  
> I use Dropbox and the MKLINK dos-command to sync the Myplaces.kml fille between computers. This is how I did it (for Windows 7):
> 
> - close GE in case it is running
> 
> - make a Google Earth subdir in your Dropbox folder. For example: "C:\Users\[your user-id]\AppData\LocalLow\Dropbox\GoogleEarth\"
> 
> - IMPORTANT: the Dropbox subdir MUST be on the same drive as the original GE subdir!
> 
> - Windows 7: go to "C:\Users\[your user-id]\AppData\LocalLow\Google\GoogleEarth"
> - copy Myplaces.kml to the Dropbox folder "C:\Users\[your user-id]\AppData\LocalLow\Dropbox\GoogleEarth\"
> - make a backup of your Myplaces.kml and store it in a safe location as a backup in case you screw up
> - delete Myplaces.kml in "C:\Users\[your user-id]\AppData\LocalLow\Google\GoogleEarth"
> - go to the Start menu, type CMD in the search box, do NOT hit enter
> - right-click CMD.EXE and click on 'run as administrator'. you will now get the DOS box
> - type MKLINK /H "C:\Users\[your user-id]\AppData\LocalLow\Google\GoogleEarth\myplaces.kml" "C:\Users\[your user-id]\AppData\LocalLow\Dropbox\GoogleEarth\myplaces.kml"
> 
> - the creation of a file hard link is confirmed
> 
> - type EXIT to close the DOS box 
`  
