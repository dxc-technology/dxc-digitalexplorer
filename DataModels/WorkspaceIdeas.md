## Workspaces Open Ideas metamodel

![image](images/Workspace.ideas.png)<br>

### **Node Definitions**

All nodes are shared with Roadmap Module

#### Relationships

|Source|Destination|Name|Properties|
|----|----|----|----|
|ClientIdea|WorkspaceGroup|ASSOCIATED_TO|
|ClientIdea|ClientDisruptor|ASSIGNED|
|Goal|WorkspaceGroup|ASSOCIATED_TO|
|KPI|WorkspaceGroup|ASSOCIATED_TO|
|ClientIdea|Goal|ADDRESSES
|ClientIdea|KPI|ADDRESSES
|ClientDisruptor|BusinessTrend|SPECIALIZES
|ClientDisruptor|TechnologyTrend|SPECIALIZES
|BusinessTrend|Workspace|REFERENCED
|TechnologyTrend|Workspace|REFERENCED
|Workspace|WorkspaceGroup|MEMBER_OF


## Change log

| Date | By | Description
|---|---|---|
|May 2020| David Stevens | First version
