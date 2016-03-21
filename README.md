# gsms_plan
Planing Document for Global Strategy Management System

## Data Vidualization / Dashboard
* Map view using [Mapbox](https://www.mapbox.com/) and [its open source libs](https://github.com/mapbox)
* Table View using [handsontable](https://github.com/handsontable/handsontable) with [Fixed Header Row and Columns](http://docs.handsontable.com/0.15.1/demo-fixed-rows-and-columns.html)


## Global Domain management
For example there is nyc.domain.com, domain.nyc, domain.com/nyc nyc.domain.com can be set as prime, and others can be redirected to prime.
The geographic region can be continent, country, city, etc.

### Integration 
* [Google Apps Admin Settings API](https://developers.google.com/admin-sdk/admin-settings/#audience) can be used to create new email accounts under google apps emails.
* [weppos/whois](https://github.com/weppos/whois) can be used to query whois info
* DNSimple's API for [tld lists](https://developer.dnsimple.com/v2/tlds/#list) and [registaring domain](https://developer.dnsimple.com/v2/registrar/#register) can be used with [dnsimple-ruby](https://github.com/aetrion/dnsimple-ruby)

## Geographical Statistics
Making global strategy requires setting priority and selecting specific geographical locations. Various statistics such as poplulation, GDP, number of companies or schools related with a specific industry is essential factor to decide priority.
### Data Format
* [GEOJSON](http://geojson.org/geojson-spec.html) with [Java](https://github.com/geotools/geotools/tree/master/modules/unsupported/geojson/src/main/java/org/geotools/geojson), or [PHP](https://github.com/jmikola/geojson)
### Data Source
* [World Bank Data API](http://data.worldbank.org/developers)

## Global Project Management
Manage projects especially (Web Development Projects), its progress, status, assignee
### Integration
* [Taiga](https://taiga.io/) with [its REST API](https://taigaio.github.io/taiga-doc/dist/api.html) and [Docker Containers](https://github.com/benhutchins/docker-taiga-example)

## Global Ticket System
### Integration
* [OTRS](https://github.com/OTRS/otrs) [its Javascript API](https://otrs.github.io/doc/api/otrs/6.0/JavaScript/index.html) and [its Docker container](https://github.com/juanluisbaptiste/docker-otrs)
* [zendesk](https://www.zendesk.com/) with [its API](https://developer.zendesk.com/rest_api/docs/core/introduction)


## User account management
Users of this software can be CEO, CFO, Sysadmins, Programmers, Designers, Contents Creators, and Translators.

### Integration
* [Google Apps Directory API](https://developers.google.com/admin-sdk/directory/) can be used for create, syncronize users from/to Google Apps

## Data Input / Data pipeline
* [huginn](https://github.com/cantino/huginn) can be used for this
