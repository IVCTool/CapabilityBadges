# ETR Interoperability Capability Badge (ETR CB)

## Interoperability Requirements

|Id|Qualifier|Requirement|Type|Test|
|---|---|---|---|---|
|ETR00001|SuT|SuT shall comply with all requirements associated with the NETN CB|Dependency||	
|ETR00002|SuT receives entity tasking|SuT shall publish the `NETN-SMC` `BaseEntity.SupportedActions` attribute.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|	
|ETR00003|SuT receives entity tasking|SuT shall publish the `NETN-SMC` `SMC_Response` interaction class.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|	
|ETR00004|SuT receives entity tasking|SuT shall publish the `NETN-ETR` `ETR_TaskStatus` interaction class.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|
|ETR00005|SuT receives entity tasking|SuT shall publish `NETN-ETR` `BaseEntity` attributes `PlannedTasks`, `CurrentTasks` and `TaskProgress`.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|
|ETR00006|SuT sends entity tasking|SuT shall publish all `NETN-ETR` `SMC_EntityControl.Task` interaction subclasses corresponding to the supported `NETN-SMC` `EntityControlActions` as declared in CS.|Declaration Management|org.nato.netn.etr.TC_ETR_0002|	
|ETR00007|SuT sends reports|SuT shall publish all `NETN-ETR` `ETR_Report` interaction subclasses as declared in CS.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|	
|ETR00008|SuT receives entity tasking|SuT shall subscribe to all `NETN-ETR` `SMC_EntityControl.Task` interaction subclasses corresponding to the supported `NETN-SMC` `EntityControlActions` as declared in CS.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|	
|ETR00009|SuT receives entity tasking|SuT shall subscribe to `NETN-ETR` `SMC_EntityControl.RequestTaskStatus` interaction class.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|	
|ETR00010|SuT receives entity tasking|SuT shall subscribe to `NETN-ETR` `SMC_EntityControl.CancelTasks` interaction class.|Declaration Management|org.nato.netn.etr.TC_ETR_0001|
|ETR00011|SuT sends entity tasking|SuT shall subscribe to the `NETN-SMC` `BaseEntity.SupportedActions` attribute.|Declaration Management|org.nato.netn.etr.TC_ETR_0002|	
|ETR00012|SuT sends entity tasking|SuT shall subscribe to the `NETN-SMC` `SMC_Response` interaction class.|Declaration Management|org.nato.netn.etr.TC_ETR_0002|	
|ETR00013|SuT sends entity tasking|SuT shall subscribe to the `NETN-ETR` `ETR_TaskStatus` interaction class.|Declaration Management|org.nato.netn.etr.TC_ETR_0002|	
|ETR00014|SuT receives reports|SuT shall subscribe to all `NETN-ETR` `ETR_Report` interaction subclasses as declared in CS.|Declaration Management|org.nato.netn.etr.TC_ETR_0002|	
|ETR00015|SuT receives entity tasking|SuT shall update the `NETN-SMC` `BaseEntity.SupportedActions` attribute to include the list of currently supported tasks.|Object Management|org.nato.netn.etr.TC_ETR_0001|
|ETR00016|SuT receives entity tasking|SuT shall respond to `NETN-ETR` `SMC_EntityControl.Task` interaction with a `NETN-SMC` `SMC_Response` with a status indicating success (accepting a task request) or failure (request not accepted).|Object Management	|org.nato.netn.etr.TC_ETR_0001|
|ETR00017|SuT receives entity tasking|SuT accepting a task request shall send `NETN-ETR` `ETR_TaskStatus` interactions to indicate changes in task execution status.|Object Management|org.nato.netn.etr.TC_ETR_0001|	
|ETR00018|SuT receives entity tasking|SuT accepting a task request shall respond to `NETN-ETR` `SMC_EntityControl.RequestTaskStatus` interaction by sending a `NETN-ETR` `ETR_TaskStatus` interaction with the latest execution status.|Object Management	|org.nato.netn.etr.TC_ETR_0001|
|ETR00019|SuT receives entity tasking|SuT accepting a task request shall update the `NETN-ETR` `BaseEntity` attributes `PlannedTasks`, `CurrentTasks` and `TaskProgress` to reflect current task status.|Object Management	|org.nato.netn.etr.TC_ETR_0001|
|ETR00020|SuT sends entity tasking|SuT shall only send `NETN-ETR` `SMC_EntityControl.Task` to an entity with a `NETN-SMC` `BaseEntity.SupportedActions` attribute value that includes the corresponding task entity control action.|Object Management	|org.nato.netn.etr.TC_ETR_0002|


## Conformance Statement

|Qualifier|Statement|Datatype|Semantics|
|---|---|---|---|
|SuT|SuT sends entity tasking|boolean||
|SuT|SuT receives entity tasking|boolean||
|SuT|SuT sends reports|boolean||
|SuT|SuT receivs reports|boolean||
|SuT sends entity tasking|Supported NETN-SMC EntityControlActions|list|1 task minimum|
|SuT sends receives tasking|Supported NETN-SMC EntityControlActions|list|1 task minimum|
|SuT sends reports|Supported NETN-SMC EntityControlActions|list|1 task minimum|
|SuT receivs reports|Supported NETN-SMC EntityControlActions|list|1 task minimum|


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


