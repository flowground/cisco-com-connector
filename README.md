# ![LOGO](logo.png) Cisco PSIRT openVuln **flow**ground Connector

## Description

A generated **flow**ground connector for the Cisco PSIRT openVuln API (version 0.0.3).

Generated from: https://api.apis.guru/v2/specs/cisco.com/0.0.3/swagger.json<br/>
Generated at: 2019-05-07T17:39:57+03:00

## API Description

The Cisco Product Security Incident Response Team (PSIRT) openVuln API is a RESTful API that allows customers to obtain Cisco Security Vulnerability information in different machine-consumable formats. APIs are important for customers because they allow their technical staff and programmers to build tools that help them do their job more effectively (in this case, to keep up with security vulnerability information).
For more information about the Cisco PSIRT openVuln API visit https://developer.cisco.com/site/PSIRT/discover/overview

For detail steps on how to use the API go to:https://developer.cisco.com/site/PSIRT/get-started/getting-started.gsp

This is a beta release of a swagger YAML for the Cisco PSIRT openVuln API

To access the API sign in with your Cisco CCO account at http://apiconsole.cisco.com and register an application
to recieve a client_id and a client_secret

You can then get your token using curl or any other method you prefer.

'curl -s -k -H "Content-Type: application/x-www-form-urlencoded" -X POST -d "client_id=<your_client_id>" -d "client_secret=<your_client_secret>" -d "grant_type=client_credentials" https://cloudsso.cisco.com/as/token.oauth2'

You will receive an access token as demonstrated in the following example:
 '{"access_token":"I7omWtBDAieSiUX3shOxNJfuy4J6","token_type":"Bearer","expires_in":3599}'

In Swagger, click on Change Authentication

enter the text "I7omWtBDAieSiUX3shOxNJfuy4J6" (which is the token you received)

then click on "Try this operation"


## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Used to obtain an advisory in CVRF format for a given advisory ID `advisory_id` (i.e., cisco-sa-20150819-pcp)

#### Input Parameters
* `advisory_id` - _required_ - advisory ID

### Used to obtain all advisories in Common Vulnerability Reporting Format (CVRF). For more information about CVRF go to https://communities.cisco.com/docs/DOC-63156 . By default the output is in JSON. To obtain the output in XML use the .xml extension. For example, /advisories/cvrf/all.xml

### Used to obtain an advisory in CVRF format for a given Common Vulnerability Enumerator (CVE). The `cve_id` format is CVE-YYYY-NNNN. For more information about CVE visit http://cve.mitre.org/

#### Input Parameters
* `cve_id` - _required_ - CVE Identifier (i.e., CVE-YYYY-NNNN)

### Used to obtain all the latest security advisories in CVRF format given an absolute number. For instance, the latest 10 or latest 5.

#### Input Parameters
* `number` - _required_ - An absolute number to obtain the latest security advisories.

### Used to obtain all the advisories that affects the given product name.

#### Input Parameters
* `product` - _required_ - An product name to obtain security advisories that matches given product name.

### Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format.

#### Input Parameters
* `severity` - _required_ - Critical, High, Medium, Low
    Possible values: critical, high, medium, low.

### Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format and additionally filter based of firstpublished start date and enddate

#### Input Parameters
* `severity` - _required_ - Used to obtain all advisories that have a security impact rating of critical
    Possible values: critical, high, medium, low.
* `startDate` - _required_
* `endDate` - _required_

### Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in CVRF format.

#### Input Parameters
* `severity` - _required_ - Used to obtain all advisories that have a security impact rating of critical
    Possible values: critical, high, medium, low.
* `startDate` - _required_
* `endDate` - _required_

### Used to obtain all security advisories that have were orginally published in a specific year `YYYY`.

#### Input Parameters
* `year` - _required_ - The four digit year.

### Used to obtain all advisories that affects the given ios version

#### Input Parameters
* `version` - _required_ - IOS version to obtain security advisories

### Used to obtain all advisories that affects the given ios version

#### Input Parameters
* `version` - _required_ - IOS version to obtain security advisories

### Used to obtain OVAL definitions for a given advisory ID `advisory_id` (i.e., cisco-sa-20150819-pcp)

#### Input Parameters
* `advisory_id` - _required_ - advisory ID

### Used to obtain all Open Vulnerability and Assessment Language (OVAL) definitions available for Cisco security vulnerabilities. For more information about OVAL go to https://communities.cisco.com/docs/DOC-63158 . By default the output is in JSON. To obtain the output in XML use the .xml extension. For example, /advisories/oval/all.xml

### Used to obtain OVAL definitions for a given CVE Identifier. The `cve_id` format is CVE-YYYY-NNNN.

#### Input Parameters
* `cve_id` - _required_ - CVE Identifier (i.e., CVE-YYYY-NNNN)

### Used to obtain all the latest OVAL definitions given an absolute number. For instance, the latest 10 or latest 5.

#### Input Parameters
* `number` - _required_ - The latest OVAL definitions (absolute number).

### Used to obtain all the oval advisories that affects the given product name.

#### Input Parameters
* `product` - _required_ - An product name to obtain security advisories that matches given product name.

### Used to obtain all OVAL definitions for a given security impact rating (critical, high, medium, or low).

#### Input Parameters
* `severity` - _required_ - Used to obtain all OVAL definitions for advisories that have a security impact rating of critical
    Possible values: critical, high, medium, low.

### Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in OVAL format.

#### Input Parameters
* `severity` - _required_ - Critical, High, Medium, Low
    Possible values: critical, high, medium, low.
* `startDate` - _required_
* `endDate` - _required_

### Used to obtain all security advisories for a given security impact rating (critical, high, medium, or low) in OVAL format.

#### Input Parameters
* `severity` - _required_ - Critical, High, Medium, Low
    Possible values: critical, high, medium, low.
* `startDate` - _required_
* `endDate` - _required_

## License

**flow**ground :- Telekom iPaaS / cisco-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
