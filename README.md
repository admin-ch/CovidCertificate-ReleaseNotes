
# Release overview
## History
|release|environment|date|note|
|----|----|----|----|
|[2.10.0](https://github.com/admin-ch/CovidCertificate-ReleaseNotes#210x)|test|01.12.2021@12:18|:rocket:|
|[2.9.9](https://github.com/admin-ch/CovidCertificate-ReleaseNotes#29x)|prod|30.11.2021@02:02|:rocket:|
|[2.9.9](https://github.com/admin-ch/CovidCertificate-ReleaseNotes#29x)|test|26.11.2021@11:41||

:rocket: : currently deployed
## Planned
|environment|release|date|
|----|----|----|
|test|-|-|
|prod|[2.10.0](https://github.com/admin-ch/CovidCertificate-ReleaseNotes#210x)|05.12.2021@00:00-00:45|

# 2.10.x
* In-app light certificate QR-Code maximal duration is reduced from 48h to 24h.
* Rapid-test based Test-Certificate validity is reduced from 48h to 24h. 
#### Services release details
|service|release|last modified|
|----|----|----|
|light-certificate-generation-service|[2.10.0](https://github.com/admin-ch/CovidCertificate-Light-Certificate-Generation-Service/releases/tag/2.10.0)|01.12.2021@15:12|

# 2.9.x
* New vaccination certificate for tourists (interfaces: UI/[CSV](https://github.com/admin-ch/CovidCertificate-UIdoc)/[API](https://github.com/admin-ch/CovidCertificate-Apidoc))
* Recovery (antibody test positive) certificate can only be generate with sample date >= 16.11.2021)
* The PDF is compatibel to the Swiss Confederation documentation style guide.
#### Services release details
|service|release|last modified|
|----|----|----|
|api-gateway-service|[2.9.2](https://github.com/admin-ch/CovidCertificate-Api-Gateway-Service/releases/tag/2.9.2)|25.11.2021@11:51|
|management-service|[2.9.7](https://github.com/admin-ch/CovidCertificate-Management-Service/releases/tag/2.9.7)|26.11.2021@11:41|
|management-ui|[2.9.5](https://github.com/admin-ch/CovidCertificate-Management-UI/releases/tag/2.9.5)|26.11.2021@08:28|

# 2.8.x
### APPS

#### Android
##### COVID Certificate
- Warning message if Covid Cert App is incorrectly used to bulk check Covid certificates.
Verification rules adapted: New and existing certificates of recovery (based on positive PCR test) now have a validity of 365 days after the start of vaccination protection in Switzerland. Existing certificates inside the app, in the form of an electronic document or on paper do not need to be reissued, because their validity is calculated at the time of testing. The testing rules abroad generally limit the use of Covid certificates to a maximum of 180 days.
- Prepared for new recovery certificates based on positive antibody tests (seropositive), which can be carried out and issued by approved laboratories starting 16.11.2021.
- Certificates which are valid and verifiable only in Switzerland display a corresponding information.
- Covid Cert App and Covid Check App (for verifiers) are more resistant to temporary failures of the EU gateway serving the mutual provision of national verification keys.
- Incorrectly displayed validities in case of deviations of the system time from the local time have been corrected.
- Further optimisations, translations and bug fixes.
##### COVID Certificate Check
- Verification rules adapted: All recovery certificates (based on a positive PCR test) now are valid for 365 days after the start of vaccination protection. Existing certificate documents (paper or PDF) with a fixed "valid until" date of less than 180 days after vaccination protection can now also be verified as being valid during the extended 365-day period, because the validity is only calculated during verification and starting from the day of vaccination.  
- Prepared for verifying the new certificates of recovery based on positive antibody tests (seropositive), which can be conducted and issued by approved laboratories starting 16.11.2021.
- Covid Cert App and Covid Check App (for verifiers) are more resistant to temporary downtimes of the EU gateway serving the mutual provision of national verification keys.
- Further optimisations, translations and bug fixes.
#### iOS
##### COVID Certificate
- Warning message if Covid Cert App is incorrectly used to bulk check Covid certificates.
Verification rules adapted: New and existing certificates of recovery (based on positive PCR test) now have a validity of 365 days after the start of vaccination protection in Switzerland. Existing certificates inside the app, in the form of an electronic document or on paper do not need to be reissued, because their validity is calculated at the time of testing. The testing rules abroad generally limit the use of Covid certificates to a maximum of 180 days.
- Prepared for new recovery certificates based on positive antibody tests (seropositive), which can be carried out and issued by approved laboratories starting 16.11.2021.
- Certificates which are valid and verifiable only in Switzerland display a corresponding information.
- Covid Cert App and Covid Check App (for verifiers) are more resistant to temporary failures of the EU gateway serving the mutual provision of national verification keys.
- Incorrectly displayed validities in case of deviations of the system time from the local time have been corrected.
- Further optimisations, translations and bug fixes.
##### COVID Certificate Check
- Verification rules adapted: All recovery certificates (based on a positive PCR test) now are valid for 365 days after the start of vaccination protection. Existing certificate documents (paper or PDF) with a fixed "valid until" date of less than 180 days after vaccination protection can now also be verified as being valid during the extended 365-day period, because the validity is only calculated during verification and starting from the day of vaccination.  
- Prepared for verifying the new certificates of recovery based on positive antibody tests (seropositive), which can be conducted and issued by approved laboratories starting 16.11.2021.
- Covid Cert App and Covid Check App (for verifiers) are more resistant to temporary downtimes of the EU gateway serving the mutual provision of national verification keys.
- Further optimisations, translations and bug fixes.
### [API](https://ws.covidcertificate.bag.admin.ch)
- New endpoint for certificate based on positive antibody test (only valid in Switzerland).
- 'Covaxin' is accepted as medicinalProductCode for the establishment of vaccination certificate. 
### [Web management UI](https://www.covidcertificate.admin.ch/)
- New menu for certificate based on positive antibody test (only valid in Switzerland).

## Release 20211002 - Saturday, October 2nd 2021

### APPS

#### Android
##### COVID Certificate
- Performance of QR code scanner optimised
- Further improvements and bug fixes
##### COVID Certificate Check
- Performance of QR code scanner optimised
- Integration of external hardware scanners
- Further improvements and bug fixes
#### iOS
##### COVID Certificate
- Further improvements and bug fixes
##### COVID Certificate Check
- Further improvements and bug fixes

### [API](https://ws.covidcertificate.bag.admin.ch)
- Vaccination and Recovery certificates are restricted to Switzerland as country of vaccination (**countryOfVaccination: 'CH'**) or test (**countryOfTest: 'CH'**).

### [Web management UI](https://www.covidcertificate.admin.ch/)

- New vaccine products.
- Generate multiple certificates (CSV): Vaccination and Recovery certificates are restricted to Switzerland as country of vaccination or test. Vaccination certificates are restricted to medicinalProductCode EU/1/20/1507, EU/1/20/1525, EU/1/20/1528.

## Release 20210913 - Monday, September 13th 2021

### APPS

- Bugfixing

### [API](https://ws.covidcertificate.bag.admin.ch)

- ValueSet-API
- Optimizations
- Bugfixing

### [Web management UI](https://www.covidcertificate.admin.ch/)

- New ValueSet for Rapid tests
- Bugfixing

## Release 20210823 - Monday, August 23th 2021

### APPS

- Bugfixing
- Language selection in the android app

### [API](https://ws.covidcertificate.bag.admin.ch)

- ValueSet-API available on TEST
- Optimizations
- Bugfixing

### [Web management UI](https://www.covidcertificate.admin.ch/)

- Bugfixing

## Release 20210809 - Monday, August 9th 2021

### APPS

- Bugfixing

### [API](https://ws.covidcertificate.bag.admin.ch)

- Bugfixing

### [Web management UI](https://www.covidcertificate.admin.ch/)

- Bugfixing

## Release 20210726 - Monday, July 26th 2021

### APPS

- Covid Cert app - AX improvement
- Covid Cert app - Certificate pdf sharing
- Covid Check app - AX improvement 
- Bugfixing

### [API](https://ws.covidcertificate.bag.admin.ch)

- Bugfixing

### [Web management UI](https://www.covidcertificate.admin.ch/)

- Bugfixing

## Release 20210712 - Monday, July 12th 2021

### APPS

- Covid Cert app - Certificate light
- Covid Check app - Certificate light support 

### [API](https://ws.covidcertificate.bag.admin.ch)

- EU Gateway connected since 08.07.2021
- Bugfixing

### [Web management UI](https://www.covidcertificate.admin.ch/)

- Bugfixing

## Release 20210628 - Monday, June 28th 2021

### APPS

- Covid Cert app InApp delivery
- Covid Cert app PDF import

### [API](https://ws.covidcertificate.bag.admin.ch)

- [InApp delivery API](https://github.com/admin-ch/CovidCertificate-Apidoc#transfer-data) to deliver Covid certificate securely and directly to the Covid Cert app

### [Web management UI](https://www.covidcertificate.admin.ch/)

- [Print](https://github.com/admin-ch/CovidCertificate-Apidoc#address-data) or [InApp](https://github.com/admin-ch/CovidCertificate-Apidoc#transfer-data) delivery can be selected for Covid certificates delivery
- CSV Upload to create several covid certificates - [Doc](https://github.com/admin-ch/CovidCertificate-UIdoc)

## Release 20210621 - Monday, June 21th 2021

### APPS

- Covid Cert app uses Verification API
- Covid Check app uses Verification API

### [API](https://ws.covidcertificate.bag.admin.ch)

- Printing API to send covid certificates per Post
- Verification API to deliver EU trust list, revocation list and business rules 

### [Web management UI](https://www.covidcertificate.admin.ch/)

- CSV Upload (BETA) to create several covid certificates - [Doc](https://github.com/admin-ch/CovidCertificate-UIdoc)

### [Covid Certificate Form](https://covidcertificate-form.admin.ch/)

- CSV Upload to generate SMS notification for the users for whom no certificate can be issued

## Release 20210614 - Monday, June 14th 2021

### [API](https://ws.covidcertificate.bag.admin.ch)

- Covid Certificate API (generation & revocation)

### [Web management UI](https://www.covidcertificate.admin.ch/)

- Bugfixing

### [Covid Certificate Form](https://covidcertificate-form.admin.ch/)

- COVID certificate application form for people who have recovered 

## Release 20210607 - Monday, June 7th 2021

### APPS

- Covid Cert app (store covid certificates)
- Covid Check app (verify covid certificates)

### API - Pilot

- Covid Certificate API (generation & revocation)

### [Web management UI](https://www.covidcertificate.admin.ch/)

- Covid Certificate Web management UI (generation & revocation and generation of OneTime password)

## Release 20210528 - Friday, May 28th 2021

### API - TEST

- Remove attribute "date and time test result" for test covid certificate due to EU specification change
- Add revocation API
- New UVCI prefix: urn:uvci:
- Bug fixes

### Web Management UI - TEST

- Remove attribute "date and time test result" for test covid certificate due to EU specification change
- Bug fixes
