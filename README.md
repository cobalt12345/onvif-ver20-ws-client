# Client for ONVIF compatible devices (IP and Term cameras, Door locks, etc.)

ONVIF is a global and open industry forum with the goal of facilitating the development and use of a global open 
standard for the interface of physical IP-based security products.

ONVIF compatible devices must support specified SOAP-XML web service interface, which is defined by set of 
WSDL (Web Services Description Language) files.

Conformance for the concrete device can be checked [here](https://www.onvif.org/conformant-products/).

All required WSDLs and XML schema files can be downloaded from [here](https://www.onvif.org/profiles/specifications/).

## How-To Build the Library

1. _download_wsdl.sh_ script lists all required files, that are actual at the moment - 06.09.2023.
It can be used to download required descriptors.
```shell
./download_wsdl.sh
```



3rd party schema files (W3C, Oasis) and catalog file were taken from another GitHub project - 
[onvif-wsdl2java](https://github.com/alzybaad/onvif-wsdl2java)

[fpompermaier/onvif](https://github.com/fpompermaier/onvif) - GitHub project, that was used as an example.

2. Generate and compile client classes:
```shell 
   mvn clean install
```