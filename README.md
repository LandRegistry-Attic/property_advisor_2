# Property Advisor, team 2

This is a Node-RED flow set which creates a map aroudn a particular property and pulls in relevant data from APIs to provide more information.

## Installing
Create a Node-RED instance, either in bluemix or otherwise (see https://nodered.org/docs/getting-started/ for tips).

Import flows_search.json and flows_information.json to separate tabs. (i.e. open in an editor, select-all, copy. Then in a Node-RED editor window click the hamburger menu, select import, from clipboard and paste.)

The flows require a key for invoking the Ornance Survey APIs.  In the flows we achieved this by placing them in the associated Cloudant database (since we're running in Bluemix)

## Running
When running, go to http://<base-url>/ui to see the app, you can enter an address and it'll switch to the property information view to show you the map with more information. It currently assumes that you didn't typo the address, if you did you need to click on the left-hand tab selector and go back to the "search" tab to re-enter.

There is currently no real interactivity, other than browsing the map!

## Modifying.
When running, you can go to http://<base-url>/red to visit the editor. To save these back to git do a select-all, then click on the hamburger menu, select export, select clipboard, select formatted and then click export. Then paste into the flows file and update git as normal.

(Better git integration is likely to come to Node-RED in the near future)