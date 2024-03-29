# Project Summary

## Project Objective/Goal

This project is a web application targeted for the use by residential real estate buyers. The application accepts the address of a property and a member id, the member id is issued to a Realtor with a subscription to the service, and the id is distributed to their clients for their use. Once a valid address and member id is submitted, the application returns details relevant for a buyer, including: property details, city summary, city crime rate/statistics, neighbourhood school rankings, and local amenities.

## Steps To Run Project

1. Navigating to the project directory
2. Start local mongodb with database named "MN_greaterVancouver"(default port, 27017)
3. Start the Node server (node app.js)
4. Connect in browser with: localhost:3000

## Technology Stack

### Web Application
- Linux, NodeJS server, MongoDB, Javascript
Dependencies:
- NodeJS: navigate to project directory, use "npm list"

## Features
General:
- Capability of comparing two locations, one by given address and another by city
Overview Tab:
- Catchment schools of each type and their rankings
- Select criminal activity stats. Compare to overal average of cities in the province?
- Nearest stores, gyms, and shopping center

School Tab:
- assigned (catchment) primary and secondary school of address (primary, secondary, early french immersion, late french immersion, secondary french immersion)
- school ranking (primary, secondary, early french immersion, late french immersion, secondary french immersion)
- assigned primary and secondary school of address
  - https://mybaragar.com/index.cfm?event=page.SchoolLocatorPublic&DistrictCode=bc41
  - https://stackoverflow.com/questions/4423272/how-to-extract-links-and-titles-from-a-html-page (grab html attribute from searches)
- locations of all private and public schools in the city
  -https://www.compareschoolrankings.org/
- school ranking
- Integrate Google Maps: Schools by type (primary, secondary, etc.) marked on map with ranking

Crime Tab:
- Vancouver Police Department
   - https://vancouver.ca/police/organization/planning-research-audit/neighbourhood-statistics.html
   - https://vpd.ca/police/organization/planning-research-audit/neighbourhood-statistics.html
- RCMP (Burnaby, Surrey, Maple Ridge, etc.)
   - http://bc.rcmp-grc.gc.ca/ViewPage.action?siteNodeId=27&languageId=1&contentId=-1
   - choose location -> select website link on (location) page -> Crime Stats & Reports
- West Vancouver
   - https://westvanpolice.ca/
   - no stats on website, found old tweet with stats: check assets folder
- Stats Canada
   - https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=3510017701&pickMembers%5B0%5D=1.1&pickMembers%5B1%5D=2.1&cubeTimeFrame.startYear=2015&cubeTimeFrame.endYear=2019&referencePeriods=20150101%2C20190101
   - https://www12.statcan.gc.ca/census-recensement/2016/dp-pd/prof/search-recherche/lst/results-resultats.cfm?Lang=E&TABID=1&G=1&Geo1=&Code1=&Geo2=&Code2=&GEOCODE=59&type=0
- Compare Location Stats tool (compare Burnaby to Vancouver)
- Integrate Google Maps: Choose location to compare via map

Local Ammenities Tab:
- Integrate Google Maps: local goccery stores, shopping centers, gyms, etc.
- Local events? Perhaps using city website to rip from events page
