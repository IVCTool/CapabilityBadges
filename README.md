# Definitions

* A **Capability** is defined by the set of **Requirements** it realizes.
* A **System** exhibits a capability when it implements all capability requirements.
* A **System under Test (SuT)** is a system undergoing testing for compliance with capability requirements.
* A **Cabability Badge** is a token of achievement awarded to a system for successfully passing testing of all capability requirements.
* **Interoperability Capability** is a capability related to a system's ability to interoperate with other systems.

# Interoperability Capabilities

The following Interoperability Capabilities related to simulation are defined in this repository. 

* HLA - the ability to participate in federated distributed simulation and to share data in a common synthetic environment.
* NETN - the ability to represent objects and interactions in an HLA federation according to the NETN-FOM.
* NETN-ETR - the abilty to send or receive simulation entity tasking requests or reports related to the observed status of simulated entities.
* NETN-TMR - the ability to trigger, request and acquire the responsibility of modelling a simulated entity.

Each interopability capability is defined by a set of requirements. Addtional required SuT information is defined in the form of a Conformance Statement (CS) template. 

## Interoperability Requirements

Each requirement has:
- a unique 8 character Identifier.
- a qualifier to determine applicability of the requirement based on SuT role
- the requirement text
- a type specifying if the requirement is referring to another set of capability requirements (Dependency), if it is a requirement related to Documentation of the SuT or if the requirement is related to any of the HLA service groups.
- a test method specifying how the requirement is expected to be verified and can either be Self Declaration or IVCT Test Report.

**Example:**

|Id|Qualifier|Requirement|Type|Test|
|---|---|---|---|---|
| CAP00005 | SuT updates X | The SuT shall publish `X` object class. |Declaration Management|IVCT Test Report|
| CAP00006 | SuT receives X | The SuT shall subscribe to `X` object class. |Declaration Management|IVCT Test Report|
| CAP00007| SuT updates X | The SuT shall use at least one of the dead-reckoning algorithms defined in CS. |Object Management|IVCT Test Report|
| CAP00008| SuT receives X | The SuT shall support all dead-reckoning algorithms as defined in CS. |Object Management|Self Declaration|



## Conformance Statement
The conformance statement template is used to capture information about the SuT relevant in order to qualify requirements.

|Qualifier|Statement|Datatype|Semantics|
|---|---|---|---|
|SuT|SuT updates X|boolean||
|SuT|SuT receives X |boolean||
|SuT updates X |DR-Algorithm|list|list of supported dead-reckoning algorithms|
|SuT receives X |DR-Algorithm|list|list of supported dead-reckoning algorithms|
