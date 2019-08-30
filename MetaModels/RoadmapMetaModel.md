
![AgendaModel](../images/RoadmapModel.png)

#### **Node Definitions**

##### Node Label: Account

|Property|Description|
|----|----|
|id|system generated
|name | Name of the Account **Required**


##### Node Label: InnovationAgenda

|Property|Description|
|----|----|
|id|system generated
|text| Short name of the agenda **Required**
|description| extended description of the innovation agenda **Required**
|creationDate| system generated - creation date of the agenda **Required**
|validUntil| user input - valid until date **Required**

##### Node Label: ClientValueChain

|Property|Description|
|----|----|
|id|system generated
|name| Name of the client value chain **Required**
|Description| extended description of the client value chain
|businessArea| pick-list - associated business area from the DE trend model
|notes | free text to add notes


##### Node Label: AgendaGoal

|Property|Description|
|----|----|
|id|system generated
|name|short text of the business goal
|Description| extended description of the business goal

##### Node Label: KPI

|Property|Description|
|----|----|
|id|system generated
|name|short description of the KPI
|measure|associated measure for the KPI


##### Node Label: Stakeholder

|Property|Description|
|----|----|
|id|system generated
|name| name of the stakeholder
|email| email address of the stakeholder

##### Node Label: ClientDisruptor

Specialized instance of the business or technology trend within the innovation agenda

|Property|Description|
|----|----|
|id|system generated
|Name|short description of the disruptor, can be changed
|description|extended description of the disruptor, can be changed
|businessArea|picklist - defines the business area this disruptor is impacting
|segment|location within the agenda Q1-Y3+
|trendType|system generate for catalog trends, picklist for signals - reference to the type of disruptor BUSINESS or TECHNOLOGY
|innovationLevel|picklist - defines the innovation level associated to this disruptor and the client
|focusArea|flag to set the value if the disruptor becomes a focus area for the account team


##### Node Label: ClientIdea
Outcome of the innovation agenda, selected focus areas are combined to create a new project idea

|Property|Description|
|----|----|
|id|system generated
|Name|short name of the client strategic initiative
|Description|
|BusinessProblem|
|creationDate|system generated creation date
|modifiedDate|system generated last modified date
|description| extended description of the 
|SFDCID| free text to capture the SFDC id
|discover|Estimated value of the discover stage
|Pilot||Estimated value of the Pilot stage
|Prototype||Estimated value of the Prototype stage
|Production||Estimated value of the Production stage
|operation||Estimated value of the operation stage
|discoverCloseDate|Estimated completion date for Discover state
|PrototypeCloseDate|Estimated completion date for the Prototype
|PilotCloseDate|Estimated completion date for the pilot
|ProductionCloseDate|Estimated completion date for the Production 
|operationCloseDate|Estimated completion date for the Operations
|Status| `approved` or `rejected`



##### Node Label: DXCInternalProgram
Internal program group to help track the creation of innovation agendas

|Property|Description|
|----|----|
|id|system generated
|Name|short name of the internal program
|description|long description of the internal program
|starttime|start date of the program
|endtime|target completion date of the program
|isActive|boolean value is program active `true` or ` false`



#### Relationships

|Source|Destination|Name|Properties|
|----|----|----|----|
|Account|InnovationAgenda|ASSOICATED
|InnovationAgenda|ClientValueChain|ASSOICATED
|InnovationAgenda|AgendaGoal|ASSOICATED
|Person|Account|ASSIGNED|{role}
|Account|Region|ASSIGNED
|Account|SubIndustry|ACCOUNT_TO_SUBINDUSTRY
|Stakeholder|InnovationAgenda|ASSIGNED
|Stakeholder|ClientValueChain|ASSIGNED
|ClientValueChain|KPI|ASSOICATED
|ClientDisruptor|ClientValueChain|DISRUPTORS
|ClientDisruptor|BusinessTrend|SPECIALIZES
|ClientDisruptor|TechnologyTrend|SPECIALIZES
|ClientIdea|ClientDistruptor|ASSIGNED
|ClientIdea|KPI|ADDRESSES
|ClientIdea|AgendaGoal|ADDRESSES
|ClientIdea|Person|ASSIGNED |role
|ClientIdea|Person|RANKED |vote
|Account|DXCInternalProgram|MEMBER_OF


----

## Change log

| Date | By | Description
|---|---|---|
|Jan 2018| David Stevens | First version
|May 2018| David Stevens | DXCInternalProgram - allow accounts to be grouped into internal programs
|June 2018| David Stevens | updates to ClientStrategicInitiative, allow KPI's and Goals to be related to these.
|March 2019|David Stevens | Idea voting, status and owners
|August 2019 |David Stevens | Idea revenue values and estimated dates