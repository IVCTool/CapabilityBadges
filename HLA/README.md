# HLA Interoperability Capability Badge (HLA CB)

## Interoperability Requirements

|Id|Qualifier|Requirement|Type|Test|
|---|---|---|---|---|
|HLA00001|SuT|SuT interoperability capabilities shall be documented in a Conformance Statement (CS).|Documentation|Inspection|
|HLA00002|SuT|SuT CS/SOM shall be complete and valid|Documentation|Inspection|
|HLA00003|SuT|SuT shall publish all object classes attributes defined as published in CS/SOM|Declaration Management||
|HLA00004|SuT|SuT shall only publish object classes attributes defined as published in CS/SOM|Declaration Management||
|HLA00005|SuT|SuT shall publish all interaction classes defined as published is CS/SOM|Declaration Management||
|HLA00006|SuT|SuT shall only publish interaction classes defined as published is CS/SOM|Declaration Management||
|HLA00007|SuT|SuT shall subscribe to all object classes attributes defined as subscribed in CS/SOM|Declaration Management||
|HLA00008|SuT|SuT shall only subscribe to object classes attributes defined as subscribed in CS/SOM|Declaration Management||
|HLA00009|SuT|SuT shall subscribe to all interaction classes defined as subscribed in CS/SOM|Declaration Management||
|HLA00010|SuT|SuT shall only subscribe to interaction classes defined as subscribed in CS/SOM|Declaration Management||
|HLA00011|SuT|SuT shall be able to be (re-)configured to use any Runtime Infrastructure implementation compliant with the SuT HLA version and API used.|Federation Management||
|HLA00012|SuT|SuT shall be able to join a specified fedation execution.|Federation Management|||
|HLA00013|SuT|The SuT shall be able to join a federation execution as a specified Federate Type.|Federation Management||
|HLA00014|SuT|The SuT shall be able to join a federation execution with a specified Federate Name.|Federation Management||
|HLA00015|SuT|SuT shall create a federation execution before joining.|	Federation Management||
|HLA00016|SuT|SuT shall join federation with minimum set of FOM modules.|	Federation Management||
|HLA00017|SuT|SuT shall register at least one object instance for each published object class|Object Management||
|HLA00018|SuT|SuT shall update initial attribute values for each published object class attribute|Object Management||
|HLA00019|SuT|SuT shall update attribute values for each published object class attribute according to update type and condition defined in CS/FOM.	|Object Management||
|HLA00020|SuT|SuT shall provide attribute value updates for requested attributes owned by the SuT|Object Management||
|HLA00021|SuT|SuT shall send at least one interaction for each published interaction class|Object Management||	
|HLA00022|SuT|SuT shall encode all updated attribute values according to CS/SOM	|Object Management||
|HLA00023|SuT|SuT shall encode all sent interaction class parameters according to CS/SOM|Object Management||	
|HLA00024|SuT|SuT shall implement/use all HLA services as described as implemented/used in CS/SOM|||		
|HLA00025|SuT|SuT shall only implement/use HLA services as described as implemented/used in CS/SOM|||		


## Conformance Statement

|Qualifier|Statement|Datatype|Semantics|
|---|---|---|---|
|SuT|SuT supports Federate Type Configuration|boolean|Required. True if SuT supports configuration of Federate Type.|
|SuT|SuT  supports Federate Name Configuration|boolean|Required. True if SuT supports configuration of Federate Name.|
|SuT|SuT  supports HLA Evolved|boolean|Required. True if SuT supports HLA Evolved.|
|SuT|SuT  supports HLA4|boolean|Required. True if SuT supports HLA4.|


SuT is HLA Time Regulating	HLA	Y/N	Required
SuT is HLA Time Constrained	HLA	Y/N	Required
FOM (Modules)	HLA	MIM, …	Minimum set of FOM Modules loaded by SuT
SOM (Modules)	HLA	…	Minimum set of SOM Modules describing SuT HLA usage




## Abbreviations

|Abbreviation|Definition|
|---|---|
|API|Application Programming Interface|
|CS|Conformance Statement|
|FOM|Federation Object Model|
|HLA|High-Level Architecture|
|RTI|(HLA) Runtime Infrastructure|
|SOM|Simulation Object Model|
|SuT|System under Test|

## References

* IEEE 1516-2010 HLA Evolved
* IEEE 1516-2025 HLA4
