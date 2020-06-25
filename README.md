# rhies_OpenMRS1.9.11
This repository contains OpenMRS version 1.9.11 used for the RHIES project

## RHIES Project
The purpose of Rwandan Health Information Exchange System (RHIES) project is to develop a system that allows for information- exchange within electronic medical record systems and to develop linkage solutions for generating EMR data directly to HMIS in the specific use case of HIV Case based surveillance (CBS). RHIES is a set of applications that work together in the Open Health Information Exchange (OpenHIE) architecture to serve point-of-service systems, like EMRs, DHIS2, National ID database and laboratory information system.

## Build
 Build the tomcat docker image by running the command  **docker build -t  savicsorg/openmrs-tomcat1911:v1.3 .**  while in the openMRS docker folder
6. Push your image to the docker hub by running the command **docker push savicsorg/openmrs-tomcat1911:v1.3** 
,Please do not forget to change the image version

 Build the mysql docker image by running the command  **docker build -t  savicsorg/openmrs-mysql1911:v1.1 .**  while in the openMRS docker folder
6. Push your image to the docker hub by running the command **docker push savicsorg/openmrs-mysql1911:v1.1** 
,Please do not forget to change the image version

## License
Mozilla Public License 2.0

## Created and Developed By
[Savics SRL](https://savics.org)

## In Collaboration with
[Rwanda Biomedical Centre (RBC)](https://www.rbc.gov.rw/)

## Main Contributors
* Developers: Gilbert AGBODAMKOU

## Libraries We Use
The following sets forth attribution notices for third party software that may be contained in portions of this repository. We thank the open source community for all of their contributions.

* [OpenMRS](https://openmrs.org/) (License: Mozilla Public License 2.0)
