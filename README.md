# Sophos_Central_Machine_Health
This will create a health report for every machines in an MSP/EDB/Single Sophos Central console
Please follow the PDF guide
This script replaces the previous scripts Endpoint_Health_EDB_MSP and Endpoint_Health_Single_Tenant scripts into one script
Alerts have also been added to the report
The config file allows other data to be added to the report as required

v2025.23
Remove the capability column. This was not a supported field and has been removed from the API
Added code to work around missing viaLogin field in the API
Added other code to better check for fields being present
MacOS only reports the major and minor version (15.4). I am working with developement to find out why the API is not returning the 3rd decimal place (15.4.1)

Version 2025.14
Fixed the report not deleting the new processes from the report

Version 2025.12
Fixed an issue if the OS Platform key was missing
Fixed missing Mac services with spaces

v2.50
New services have been added
For MSP or EDB customers you can now turn on a menu that lists all the consoles and run a report for just one of them
Added the ability to report just machines with issues

v2.41
Fixed an issue where under some circumstances Alerts would get a 403 error

v2.40
Fixed an issue where you could see an XDR or item error
Added the option to add the sub estate ID to the report

v2.36
Added a timer to report how long the report takes
Fixed an issue where some alerts could be missed

v2.31
Fixed an issue where alerts could be over reported
Added the functionality to generate a report per sub estate rather than one big report

v2.20
Fixed an issue when the script was run against a Sophos Central Enterprise Dashboard
