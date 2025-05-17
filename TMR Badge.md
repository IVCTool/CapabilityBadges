# TMR Interoperability Capability Badge (TMR CB)

## Interoperability Requirements

|Id|Qualifier|Requirement|Type|Test|
|---|---|---|---|---|
|TMR00001|SuT|SuT shall publish the `NETN-TMR` `BaseEntity.AllocatedFederate` attribute|Declaration Management||
|TMR00002|SuT acquires modelling responsibility|SuT shall subscribe to the `NETN-TMR` `BaseEntity.AllocatedFederate` attribute|Declaration Management||
|TMR00003|SuT acquires modelling responsibility|SuT shall subscribe to the `NETN-TMR` `SMC_FederateControl.AcquireModellingResponsibility` interaction class |Declaration Management||
|TMR00004|SuT|SuT shall update owned `NETN-TMR` `BaseEntity.AllocatedFederate` object instance attributes with the `Federate Name` of the federate with the intended modelling responsibility.|Object Management||
|TMR00005|SuT acquires modelling responsibility|SuT shall invoke the `Attribute Ownership Acquisition` HLA service to request ownership of attributes including the `NETN-TMR` `BaseEntity.AllocatedFederate` attribute if the object instance attribute `NETN-TMR` `BaseEntity.AllocatedFederate` is not already owned by SuT and if the value of the attribute is equal to the SuT `Federate Name`.|Ownership Management||
|TMR00006|SuT divests modelling responsibility|SuT shall respond to HLA `Request Attribute Ownership Release` callbacks with the same set of requested attribute designators by invoking the `Attribute Ownership Divestiture If Wanted` HLA service or the `Attribute Ownership Release Denied` HLA service, i.e., no partial release of attribute ownership is allowed.|Ownership Management||
|TMR00007|SuT acquires modelling responsibility|SuT shall update |Ownership Management||




## Conformance Statement

|Qualifier|Statement|Datatype|Semantics|
|---|---|---|---|
|SuT|SuT acquires modelling responsibility|boolean||
|SuT|SuT divests modelling responsibility|boolean||







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
