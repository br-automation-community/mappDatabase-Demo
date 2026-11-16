> **Hinweis / Notice:** Please read the [Disclaimer](#disclaimer) / [Haftungsausschluss](#haftungsausschluss) at the end of this README before using this software.

## Table of Contents
* [Introduction](#Introduction)
* [Python script changes](#Script)
* [Requirements](#Requirements)
* [Revision History](#Revision-History)

<a name="Introduction"></a>
## Introduction
This is a demo application for a simple recipe managment with mappDatabase. It is not and official B&R product. See the [WIKI](https://github.com/br-automation-community/mappDatabase-Demo/wiki) for a detailed guide how to setup different SQL servers. 

![](https://github.com/br-automation-community/mappDatabase-Demo/blob/main/Wiki/screenshot.png)

<a name="Script"></a>
## Python script changes
This sample also includes a customized version of the Python script used to connect to the database server. The script is fully compatible with the B&R script. See Automation Studio help (e046127f-e239-4f17-bd17-3ae889dac782) and the [WIKI](https://github.com/br-automation-community/mappDatabase-Demo/wiki) for more details how to use the script.

#### The script changes include:
- Added more and detailed error messages
- Print all SQL queries and server response details
- Trim data type string when reading from database
- Change MsSQL database provider to 'ODBC Driver 17 for SQL Server' to support Linux systems
- Removed dependency from MySql driver for data conversion. It is no longer required to install MySQL driver when using MsSQL.

<a name="Requirements"></a>
## Requirements (current used versions)
* Automation Studio 4.9
* mapp 5.14
* Automation Runtime B4.83

Recommended task class is #8 with a 10ms cycle time. For the nettime and axis tasks use #1

<a name="Revision-History"></a>
## Revision History
You can find details in the project in "revision.txt"

#### Version 1.2 (10.02.2023)
- PythonScript: Support for MS SQL data type decimal

#### Version 1.1 (05.01.2022)
- Added script server ping
- PLC: Update to runtime E4.90 and mapp 5.16
- PythonScript: Added PLC raw data to debug output

#### Version 1.0
- First public release

# Disclaimer
* License: The source code for this software is provided in this repository under the MIT License—with the consent of the author and B&R Industrie-Elektronik GmbH, which, pursuant to Section 69b of the German Copyright Act (UrhG), is entitled to exercise the economic rights regarding the software. Third-party components are subject to their respective licenses. B&R products are not covered by this license and require a separate license.
* Not a Product: Neither the author, the repository owner, B&R Industrie-Elektronik GmbH, nor any other companies within the ABB Group sell the content provided here as a product. It is provided free of charge and not as part of any commercial business activity. The content of this repository is not maintained as a commercial software product and should not be regarded as such.
* No Support: No support is offered or provided for the program or the codebase. There is no maintenance, no ad-hoc bug fixing, no provision of updates (including security updates) or further development, and there are no guaranteed response times.
* No Warranty: The software is provided "as is"—without any express or implied warranties of any kind. The user is solely responsible for the use of the software.
* No Guarantee: No guarantees are made—specifically regarding fitness for a particular purpose, the absence of errors, the absence of third-party rights, or the completeness or accuracy of the code, its functionality, the documentation, or any other provided content.
* Liability: The liability disclaimer set forth in the MIT License applies to the fullest extent permitted by law. Mandatory statutory liability (e.g., for intent, injury to life, body, or health, or under the Product Liability Act) remains unaffected.
* Trademarks: B&R, Automation Studio, Automation Runtime, mappView, mappService, mappMotion, and Safety+ are trademarks of B&R Industrial Automation GmbH or a company within the ABB Group. No trademark rights are granted.
* In the event of any discrepancies between the German and the English version, the German version shall prevail.

# Haftungsausschluss
* Lizenz: Der Quellcode dieser Software wird in diesem Repository unter der MIT-Lizenz zur Verfügung gestellt – mit Zustimmung des Autors und der B&R Industrie-Elektronik GmbH, die gemäß § 69b UrhG zur Ausübung der vermögensrechtlichen Befugnisse an der Software berechtigt ist. Komponenten Dritter unterliegen ihren jeweiligen Lizenzen. Produkte von B&R sind nicht Gegenstand dieser Lizenz und bedürfen einer eigenen Lizenz.
* Kein Produkt: Weder der Autor, der Inhaber des Repositorys, noch die B&R Industrie-Elektronik GmbH oder andere Gesellschaften der ABB-Gruppe verkaufen die hier bereitgestellten Inhalte als Produkt. Die Bereitstellung erfolgt unentgeltlich und nicht im Rahmen einer Geschäftstätigkeit.  Die Inhalte dieses Repositorys werden nicht als kommerzielles Softwareprodukt gepflegt und sollten auch nicht als solches betrachtet werden.
* Kein Support: Für das Programm und die Codebasis wird kein Support angeboten oder geleistet. Es erfolgt keine Wartung, keine Fehlerbehebung auf Anfrage, keine Bereitstellung von Updates (einschließlich Sicherheitsupdates) oder Weiterentwicklung und es gibt keine garantierten Reaktionszeiten.
* Keine Gewährleistung: Die Software wird „wie besehen“ („as is“) bereitgestellt – ohne jegliche ausdrückliche oder stillschweigende Gewährleistung. Der Nutzer ist für die Verwendung der Software allein verantwortlich.
* Keine Garantie: Es wird keine Garantie übernommen, insbesondere nicht für die Eignung für einen bestimmten Zweck, Fehlerfreiheit oder Freiheit von Rechten Dritter, sowie die Vollständigkeit oder Richtigkeit – weder in Bezug auf den Code und dessen Funktionalität noch in Bezug auf die Dokumentation oder andere bereitgestellte Inhalte.
* Haftung: Es gilt der Haftungsausschluss der MIT-Lizenz, soweit gesetzlich zulässig. Zwingende gesetzliche Haftung (e.g. Vorsatz, Verletzung des Lebens, des Körpers oder der Gesundheit sowie nach dem Produkthaftungsgesetz)  bleibt unberührt.
* Marken: B&R, Automation Studio, Automation Runtime, mappView, mappService, mappMotion, Safety+ sind Marken der B&R Industrial Automation GmbH bzw. einem Unternehmen der ABB-Gruppe. Es werden keine Markenrechte eingeräumt.
* Im Falle von Abweichungen zwischen der deutschen und der englischen Fassung hat die deutsche Fassung Vorrang.
