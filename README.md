# Samsung-Smartthings-Custom-Rest-API
Custom Rest API for Samsung Smartthings

Web Service (Rest) for Samsung Smartthings

Installation:

1 - Connect to: https://graph.api.smartthings.com/ide/apps

2 - Click the button "New SmartApp"

3 - Select the "From Code" tab

4 - copy paste the content of the code.groovy file into the window

5 - click next: that's it, the SmartApp should be created

Usage:

1 - While in the App, click the "Publish" Button (then click "For Me")
2 - your app should now be active.. 
3 - locate your App ID and your Authorization Token:
  App ID example: ffffffff-ffff-ffff-ffff-ffffffffffff
  Authorization Token example: Bearer ffffffff-ffff-ffff-ffff-ffffffffffff
  
  => note: the App ID and Auth Token are different...
  
4 - Invoke Rest Calls:

  Type: GET
  Headers:
    Authorization: Bearer ffffffff-ffff-ffff-ffff-ffffffffffff
  https://graph.api.smartthings.com/api/smartapps/installations/<APP ID>/<End Point>

Examples of Endpoints:
  /contacts                         (get devices that have contacts attributes)
  /events/contacts                  (get all contact type events)
  /events/contacts?id=<Device ID>   (Get all Contact Events for 1 specific device)
  
  /motions
  /events/motions
  /events/motions?id=<Device ID>
  
  /locks
  /events/locks
  /events/locks?id=<Device ID>
  
  /lux
  /events/lux
  /events/lux?id=<Device ID>
  
  /colors
  /events/colors
  /events/colors?id=<Device ID>
  
  /alarms
  /events/alarms
  /events/alarms?id=<Device ID>
  
  /switches
  /events/switches
  /events/switches?id=<Device ID>
  
  /temperatures
  /events/temperatures
  /events/temperatures?id=<Device ID>
  
  /shocks
  /events/shocks
  /events/shocks?id=<Device ID>
  
 
