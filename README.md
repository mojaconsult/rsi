# RSI
"Rural Solar Innovation" is a project in Mont-Soleil. 
This git repository provides configuration information for OpenHAB 1.8 that is used as an 
insulation between the "things" in the building and the cloud.   

## Naming
We call all devices according to IoT "things". In the naming of OpenHAB such things have 
variables called "Items" 

## State of the things
### Simulation items
Most default.items are simulated (the demo.items currently still in within default.items).

### Technology- and bindig-items
enocean.items, hue.items, zwave.items are showing the currently available items we have in our office. 
astro.items and weather.items handle the respective parts of those bindings.

## Sitemaps
default.sitemap encompasses all the technology- and binging-items that work already. 
rsi.sitemap is structured according to the rsi project.
testing.sitemap provides all the items that are currently still not completely working.

### Default.sitemap bugs
The weather web snippet does not work on iPhone (not testet on Android). 
The visibility toggle for the hue bulb color picker, etc. makes the web frontend receiving unclear states ("URL ... #301").

### Technology- and bindig-items
Such sitemaps are to show the capabilities of the respective technology or binging.

## Simulation
the demo.items and rsi.items are currently simulated through demo.rules and rsi.rules.

## State of the Cloud
The cloud is planned to run on Logstash or MongoDB, Elasticsearch and Kibana. 

## Known Issues
The logging out of OpenHAB for Logstash is currently not working. 
