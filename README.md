# gsms_plan
Planing Document for Global Strategy Management System

## Data Vidualization / Dashboard
* Map view using [Mapbox](https://www.mapbox.com/) and [its open source libs](https://github.com/mapbox)
* Table View using 

## User account management
### Integration
* [Google Apps Directory API](https://developers.google.com/admin-sdk/directory/) can be used for create, syncronize users from/to Google Apps

## Geographical Statistics
Making global strategy requires setting priority and selecting specific geographical locations. Various statistics such as poplulation, GDP, number of companies or schools related with a specific industry is essential factor to decide priority.
### Data Format
* [GEOJSON](http://geojson.org/geojson-spec.html) with [Java](https://github.com/geotools/geotools/tree/master/modules/unsupported/geojson/src/main/java/org/geotools/geojson), or [PHP](https://github.com/jmikola/geojson)Taiga

## Global Project Management
Manage projects, its progress, status, assignee
### Integration
* [Taiga](https://taiga.io/) with [its REST API](https://taigaio.github.io/taiga-doc/dist/api.html) and [Docker Containers](https://github.com/benhutchins/docker-taiga-example)

## Global Domain management
For example there is nyc.domain.com, domain.nyc, domain.com/nyc nyc.domain.com can be set as prime, and others can be redirected to prime.
The geographic region can be continent, country, city, etc.

### Integration 
* [Google Apps Admin Settings API](https://developers.google.com/admin-sdk/admin-settings/#audience) can be used to create new email accounts under google apps emails.
