# gsms_plan
Planing Document for Global Strategy Management System - GSMS

## Background
[As of 2012, at least 16 International Organizations such as World Bank or UNICEF are using SAP] as their [ERP](https://en.wikipedia.org/wiki/Enterprise_resource_planning) system(https://www.ctbto.org/service/expert-area/core/interesting-facts-about-the-erp-project/). But there is other orgs not having budget big enough to purchase SAP but still need ERP for international operation. Open source ERP is usually focusing on small or middle sized business and not sutable for global organization with presence in multiple countires. GSMS project will [challenge to implement](http://panorama-consulting.com/challenges-with-international-erp-implementations/) open source global ERP to fill the gap.

## Data Vidualization / Dashboard
* Map view using [Mapbox](https://www.mapbox.com/) and [its open source libs](https://github.com/mapbox)
* Table View using [handsontable](https://github.com/handsontable/handsontable) with [Fixed Header Row and Columns](http://docs.handsontable.com/0.15.1/demo-fixed-rows-and-columns.html)
* Realtime Graph using [Grafana](https://github.com/grafana/grafana)

## Global Domain management
For example there is nyc.domain.com, domain.nyc, domain.com/nyc nyc.domain.com can be set as prime, and others can be redirected to prime.
The geographic region can be continent, country, city, etc.
* [Google Apps Admin Settings API](https://developers.google.com/admin-sdk/admin-settings/#audience) can be used to create new email accounts under google apps emails.
* [weppos/whois](https://github.com/weppos/whois) can be used to query whois info
* DNSimple's API for [tld lists](https://developer.dnsimple.com/v2/tlds/#list) and [registaring domain](https://developer.dnsimple.com/v2/registrar/#register) can be used with [dnsimple-ruby](https://github.com/aetrion/dnsimple-ruby)
* [AWS SDK for ruby](https://github.com/aws/aws-sdk-ruby)

## Geographical Statistics
Making global strategy requires setting priority and selecting specific geographical locations. Various statistics such as poplulation, GDP, number of companies or schools related with a specific industry is essential factor to decide priority.

### Data Format 
* [GEOJSON](http://geojson.org/geojson-spec.html) with [Java](https://github.com/geotools/geotools/tree/master/modules/unsupported/geojson/src/main/java/org/geotools/geojson), or [PHP](https://github.com/jmikola/geojson)

### Data Source
* [World Bank Data API](http://data.worldbank.org/developers)
* [UN Data API](http://data.un.org/Host.aspx?Content=API)

## Global Project Management
Manage projects especially (Web Development Projects), its progress, status, assignee
* [Taiga](https://taiga.io/) with [its REST API](https://taigaio.github.io/taiga-doc/dist/api.html) and [Docker Containers](https://github.com/benhutchins/docker-taiga-example)

## Global Ticket System
* [OTRS](https://github.com/OTRS/otrs) [its Javascript API](https://otrs.github.io/doc/api/otrs/6.0/JavaScript/index.html) and [its Docker container](https://github.com/juanluisbaptiste/docker-otrs)
* [zendesk](https://www.zendesk.com/) with [its API](https://developer.zendesk.com/rest_api/docs/core/introduction)

## Translation Management System
* [zanata](http://zanata.org/) and [zanata api](https://zanata.ci.cloudbees.com/job/zanata-api-site/site/zanata-common-api/rest-api-docs/index.html)
* [fake-zanata-server](https://www.npmjs.com/package/fake-zanata-server)
* [zanata docker image](https://github.com/zanata/docker-images)

## User account management
Users of this software can be CEO, CFO, Sysadmins, Programmers, Designers, Contents Creators, and Translators.
* [Google Apps Directory API](https://developers.google.com/admin-sdk/directory/) can be used for create, syncronize users from/to Google Apps

## Data Input / Data pipeline
* [huginn](https://github.com/cantino/huginn) can be used for this
