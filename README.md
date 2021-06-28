# Release notes

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
