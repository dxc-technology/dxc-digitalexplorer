# Global Meta Nodes

The following nodes provide key information to 2 or more modules within the overall Graph model.  
Changes to these have a wide ranging impact to all modules within Digital Explorer

### Updates to these nodes apply the following Roles
* Add (new) - added to both the META_ and live data nodes
* Update - updates applied to both META_ and live data nodes
* Delete - Deleted from META_ , only delete from LIVE if no relationship to other nodes are in place

## Industry & Sub-Industry
DXC industry model
<br>![image](../images/DXCAligned.png)<br>
**Node label : META_Industry**<br>
**Node label : META_SubIndustry**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
|   | X | X | X | X | X | X |


## Business Areas
3rd level of the industry model, provides details of value chains and/or key business areas relevant to Digital Transformation

**Node label : META_BusinessArea**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
|   | X | X |  | X | X |  |


## Regions
DXC region information
<br>![image](../images/DXCAligned.png)<br>
**Node label : Region**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| |  |X| X | | |

## Offering Family
DXC offering family names 
<br>![image](../images/DXCAligned.png)<br>
**Node label : META_Practice**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| |  |  | X | | X|


## DXC Delivery Centers
Master list of DXC global delivery centers

**Node label : DeliveryCenter**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| |  |  | X |X | |

## DXC Delivery Center Type
Defines the type of delivery center - examples `DTC`, `RDC`

**Node label : DeliveryCenterType**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| |  |  | X |X | |

## Roles
Master list of available roles to assign to a person

**Node label : META_PersonRole**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| | X | X | X | |X |


## Technology Groups
Master list of technology groups, where technology trends and solution features can be assigned.

**Node label : META_TechnologyGroup**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| | X |  | X | | X |

## Documentation Types
Master list of available documentation types

**Node label : META_DocumentationCategory**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| | |  | X | X |  |



## Solution Type
Top level grouping for solutions - examples `DXC Solution`, `Partner Capability`
**Node label : META_SolutionType**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| | |  |  | X |  |

## Solution Sub Type
Second level grouping for solutions, below `SolutionType` - examples `Concept`, `Pilot`
**Node label : META_SolutionSubType**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| | |  |  | X |  |

## Solution Status
Master list of available statuses for a solution
**Node label : META_Status**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| | |  |  | X |  |

## Solution Category
Optional : High-level grouping for solutions, used within internal DXC campaigns and competitions.

**Node label : META_Category**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| | |  |  | X |  |


## Solution Feature Category
Defines the type of solution features, offering, capability, method

**Node label : META_FeatureCategory**

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| | |  |  | X |  |

## Person
Reference node for all people associated with any module, action or node within the database.

**Used in**

|   | Trends| Roadmaps | Solutions | Workspaces | Explorer|Playbooks
|---|---|---|---|---|---|---|
| |X |X  | X | X |X  |
