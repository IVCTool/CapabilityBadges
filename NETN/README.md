# NETN Interoperability Capability Badge

## Interoperability Requirements

|Id|Qualifier|Requirement|Type|Test|
|---|---|---|---|---|
|NETN0001|SuT|SuT shall comply with all requirements associated with the HLA CB|Dependency||
|NETN0002|SuT|SuT shall comply with all requirements associated with at least one of the following CB: ETR, TMR|Dependency||
|NETN0003|SuT|SuT shall document in CS if the SuT is supporting HLA Evolved|Documentation|Inspection|
|NETN0004|SuT|SuT shall document in CS if the SuT is supporting HLA4|Documentation|Inspection|
|NETN0005|SuT supports HLA Evolved|SuT shall be able to connect to an HLA Runtime Infrastructure using the IEEE-1516.1-2010 (HLA Evolved) interface with any of the provided standard APIs.|Federation Management| |
|NETN0006|SuT supports HLA4|SuT shall be able to connect to an HLA Runtime Infrastructure using the IEEE-1516.1-2025 (HLA 4) interface with any of the provided standard APIs.|Federation Management||
|NETN0007|SuT|SuT shall be able to join as an HLA federate to an HLA federation execution with following loaded FOM modules:  All SISO-STD-001.1-2015 (RPR-FOM v2) FOM Modules, all AMSP-04 Ed C (NETN-FOM v4) FOM Modules.|Federation Management||
|NETN0008|SuT|SuT shall publish all required attributes for published object classes.|Declaration Management||
|NETN0009|SuT|SuT shall include all required parameters when sending interactions.|Object Management||

## Conformance Statement

|Statement|Datatype|Semantics|
|---|---|---|
|SuT supports HLA Evolved|boolean|Required. True if SuT supports HLA Evolved.|
|SuT supports HLA4|boolean|Required. True if SuT supports HLA4.|



## Abbreviations

|Abbreviation|Definition|
|---|---|
|API|Application Programming Interface|
|CB|Capability Badge|
|CS|Conformance Statement|
|FOM|Federation Object Model|
|HLA|High-Level Architecture|
|SuT|System under Test|

## References

* IEEE 1516-2010 HLA Evolved
* IEEE 1516-2025 HLA4
* SISO-STD-001
* AMSP-04 Ed C
