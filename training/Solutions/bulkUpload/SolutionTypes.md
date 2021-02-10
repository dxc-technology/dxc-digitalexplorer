# Solution Type look up table

Digital Explorer allows a solution to be categories as a certain type, demo, partner, reference architecture, etc.  the table below is the master list of solution types and their IDs to be used within the CSV loader


|SolutionSubType ID|Solution Type| Solution Sub Type|
|---|---|---|
835456|Reference DataSets |DXC Pattern 
830522|Reference DataSets |DXC Sub Offering 
802527|Reference DataSets |Client Success Story 
416565|Reference DataSets |DXC Offering Family 
416575|Reference DataSets |DXC Reference Architecture 
416566|Reference DataSets |Partner Capability 
12600|Standard Solution |DXC Demo 
9072|Standard Solution |DXC Solution 
12759|Standard Solution |DXC Labs 
432060|Accelerated Solution Development |Production 
432057|Accelerated Solution Development |Concept 
432059|Accelerated Solution Development |Pilot 
432058|Accelerated Solution Development |Prototype 
820928|Partners |Red Hat 
812795|Partners |SAP 
812793|Partners |PWC 
812791|Partners |Oracle 
812789|Partners |Microsoft 
812787|Partners |MicroFocus 
812785|Partners |Lenovo 
812783|Partners |IBM 
812798|Partners |HPE 
812796|Partners |Dell EMC / vmware 
806990|Partners |AWS 
806993|Partners |AT&T 
801897|Partners |Google 
801513|Partners |RenderMedia 
801620|Partners |ServiceNow 
801618|Partners |HPI 
801550|Partners |HCL 
801656|Partners |Hitachi 

**To request new entries to this list contact the Digital Explorer admin team**

---

~~~
match (st:META_SolutionType)--(sst:META_SolutionSubType)
return id(sst),st.name,sst.name
~~~