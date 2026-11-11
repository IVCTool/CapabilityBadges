# ETR Reporting Interoperability Capability Badge (ETR Reporting CB)

## Interoperability Requirements

|Id|Qualifier|Requirement|Type|Test|
|---|---|---|---|---|
|ETR00001|SuT|SuT shall comply with all requirements associated with the NETN CB|Dependency||	
|ETR00007|SuT sends reports|SuT shall publish all `NETN-ETR` `ETR_Report` interaction subclasses as declared in CS.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|	
|ETR00014|SuT receives reports|SuT shall subscribe to all `NETN-ETR` `ETR_Report` interaction subclasses as declared in CS.|Declaration Management|org.nato.netn.etr.TC_ETR_0002|	

## Conformance Statement

|Qualifier|Statement|Datatype|Semantics|
|---|---|---|---|
|SuT|SuT sends reports|boolean||
|SuT|SuT receivs reports|boolean||
|SuT sends reports|Supported ETR_Report classes|list|1 report minimum|
|SuT receivs reports|Supported ETR_Report classes|list|1 report minimum|

## Abbreviations

|Abbreviation|Definition|
|---|---|
|API|Application Programming Interface|
|CB|Capability Badge|
|CS|Conformance Statement|
|ETR|Entity Tasking and Reporting|
|FOM|Federation Object Model|
|HLA|High-Level Architecture|
|SMC|Simulation Management and Control|
|SuT|System under Test|

## References

* IEEE 1516-2010 HLA Evolved
* IEEE 1516-2025 HLA4
* SISO-STD-001
* AMSP-04 Ed C


