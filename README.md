# SecureX Orchestration Workflow - Umbrella Brand Watch
A workflow for automating the discovery of imposter domains to detect typosquatting, brandjacking or similar attacks.
the original idea and python version:
https://umbrella.cisco.com/blog/automating-imposter-domain-discovery
https://github.com/brad-anton/brand_watch


## Features
* Automatic Regex brand generator based on https://github.com/brad-anton/brand_watch
* Ability to exclude domains
* Queries Cisco Umbrella Investigate API with adjustable settings
* Possibility to run scheduled every day
* Possibility to feed into your SOC / SIEM / TIP / ..

 **Please always test thoroughly before using in production!**
Based on the brand you are monitoring, you can adjust the frequency and maximum results returned.

## Installation
1. Browse to your SecureX orchestration instance. This wille be a different URL depending on the region your account is in: 

* US: https://securex-ao.us.security.cisco.com/orch-ui/workflows/
* EU: https://securex-ao.eu.security.cisco.com/orch-ui/workflows/
* APJC: https://securex-ao.apjc.security.cisco.com/orch-ui/workflows/

2. Click on **IMPORT** to import the workflow.

3. Click on **Browse** and copy paste the content of the json file inside of the text window. 

4. Click on **IMPORT**. 

5. Click on **UPDATE** and fill in the Umbrella Investigate API key.

> **Note:** To obtain your Umbrella Investigate API key, please follow these steps: https://docs.umbrella.com/investigate-api/docs/about-the-api-authentication


## Notes

* Please test this properly before implementing in a production environment. This is a sample workflow!

## Author(s)

* Bart Bruninx (Cisco)
